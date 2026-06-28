[Importyeti Scraper](https://apify.com/lulzasaur/importyeti-scraper?fpr=data)

# ImportYeti Scraper

Scrape US import/export trade data from ImportYeti. Search for companies, view detailed company profiles with supplier and buyer relationships, and extract shipment records including HS codes, ports, carriers, and product descriptions.

## Features

- **Company search** -- Find importers and exporters by keyword, product, or HS code
- **Company profiles** -- Get detailed profiles including address, website, total shipments, top products, suppliers, and buyers
- **Shipment records** -- Extract individual shipment data with HS codes, weights, ports, and bill of lading numbers
- **Supplier/buyer mapping** -- Discover trade relationships between companies
- **Country filtering** -- Filter results by supplier country of origin
- **HS code filtering** -- Target specific product categories by Harmonized System code
- **JSON API + HTML fallback** -- Uses ImportYeti's internal API when available, falls back to HTML scraping
- **Pagination support** -- Automatically follows paginated search results and shipment pages

## Input Parameters

| Parameter | Type | Default | Description |
| --- | --- | --- | --- |
| `mode` | string | `"search"` | Mode: `search`, `company`, or `shipments` |
| `searchQuery` | string | `""` | Search term (company name, product keyword, or general term) |
| `companyName` | string | `""` | Company name or URL slug for `company`/`shipments` mode |
| `hsCode` | string | `""` | Filter by HS code for specific product categories |
| `country` | string | `""` | Filter by supplier country (e.g., "China", "Vietnam") |
| `limit` | integer | `50` | Maximum number of results (1-500) |
| `maxPages` | integer | `5` | Maximum pages to scrape (1-50) |
| `proxyConfiguration` | object | -- | Proxy settings (recommended to avoid rate limits) |

## Example Inputs

**Search for electronics importers:**

```
{
  "mode": "search",
  "searchQuery": "electronics",
  "country": "China",
  "limit": 50
}
```

**Get a company profile:**

```
{
  "mode": "company",
  "companyName": "nike"
}
```

**Get shipment records for a company:**

```
{
  "mode": "shipments",
  "companyName": "apple-inc",
  "hsCode": "8471",
  "limit": 100
}
```

## Output Fields

### Search Results

| Field | Type | Description |
| --- | --- | --- |
| `companyName` | string | Company name |
| `slug` | string | URL slug on ImportYeti |
| `address` | string | Company address (if available) |
| `totalShipments` | number | Total shipment count |
| `country` | string | Country of origin |
| `url` | string | ImportYeti profile URL |

### Company Profile

| Field | Type | Description |
| --- | --- | --- |
| `companyName` | string | Company name |
| `address` | string | Company address |
| `website` | string | Company website |
| `phone` | string | Phone number |
| `country` | string | Country |
| `totalShipments` | number | Total sea shipments recorded |
| `alsoKnownAs` | array | Alternate company names |
| `topProducts` | array | Top imported/exported products with HS codes |
| `hsCodes` | array | All associated HS codes |
| `suppliers` | array | Supplier names, countries, and shipment counts |
| `buyers` | array | Buyer/customer names and shipment counts |
| `recentShipments` | array | Recent shipment records |
| `carriers` | array | Shipping carriers used |
| `ports` | array | Ports used |
| `countriesOfOrigin` | array | Countries goods are sourced from |

### Shipment Records

| Field | Type | Description |
| --- | --- | --- |
| `shipmentDate` | string | Date of shipment |
| `supplierName` | string | Supplier/shipper name |
| `buyerName` | string | Buyer/consignee name |
| `productDescription` | string | Product description |
| `hsCode` | string | HS tariff code |
| `weight` | string | Shipment weight |
| `quantity` | string | Quantity shipped |
| `portOfLading` | string | Origin port |
| `portOfUnlading` | string | Destination port |
| `billOfLading` | string | Bill of lading number |
| `vesselName` | string | Vessel/ship name |
| `country` | string | Country of origin |

## Use Cases

- **Supplier discovery** -- Find overseas suppliers for any product category
- **Competitive intelligence** -- See who your competitors are importing from
- **Supply chain mapping** -- Map the full supplier and buyer network for any company
- **Trade compliance** -- Verify supplier relationships and shipment volumes
- **Sourcing research** -- Compare suppliers by shipment frequency, HS codes, and country of origin
- **Market analysis** -- Analyze import trends by product category or country

## Data Source

Data is sourced from [ImportYeti](https://www.importyeti.com/), which aggregates US customs import records and bill of lading data.

---

## Run on Apify

This scraper runs on the [Apify platform](https://apify.com/?fpr=lulzasaur) -- a full-stack web scraping and automation cloud. Sign up for a free account to get started with 30-day trial of all features.

[Try Apify free ->](https://apify.com/?fpr=lulzasaur)