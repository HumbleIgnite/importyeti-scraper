[Importyeti Scraper](https://apify.com/crawlerbros/importyeti-scraper?fpr=data)

Scrape US import/export trade data from [ImportYeti](https://www.importyeti.com). For each query, returns a list of companies / suppliers with shipment counts, most-recent-shipment date, top trading partners, trademarks, and country of operation.

## Input

| Field | Type | Description |
| --- | --- | --- |
| `query` | string | Company name, supplier name, trademark, or product keyword. Required. |
| `type` | enum | `any`, `company`, or `supplier`. |
| `mostRecentShipment` | enum | `any`, `6mo`, or `12mo` (include only companies active in the window). |
| `minShipments` | integer | Exclude companies with fewer lifetime shipments. |
| `maxResults` | integer | Max records to return (1–1000, 10 per page). |

## Output

Per record:

- `type` = `importyeti_record`
- `name` — company / supplier name
- `recordType` — `company` or `supplier`
- `countryCode` — ISO 2-letter
- `address`
- `totalShipments` — lifetime shipment count
- `mostRecentShipment` — DD/MM/YYYY of latest shipment
- `topSuppliers` — list of the top trading partners (filtered for placeholders)
- `trademarks` — list of associated trademarks (when present)
- `detailUrl` — direct link to the ImportYeti profile page
- `scrapedAt` — ISO timestamp

## How it works

- Hits `https://www.importyeti.com/api/search?q=<query>&page=<N>` (10 results/page).
- Paginates until `maxResults` is reached or no new data appears.
- All filters (`type`, `mostRecentShipment`, `minShipments`) are applied client-side because the public API ignores those parameters.
- `curl_cffi` with Chrome-131 TLS fingerprint; no cookies, no proxy required.

## FAQ

**Do I need a proxy or login?** No.
**Why are the filters applied client-side?** ImportYeti's public search API ignores filter parameters and always returns 10 mixed results per page. The actor fetches more pages than requested and filters down.