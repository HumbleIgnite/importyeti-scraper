[Importyeti Scraper](https://apify.com/parseforge/importyeti-scraper?fpr=data)

![ParseForge Banner](https://images.apifyusercontent.com/wTxwbnRh8X878EoDysptDr1AzClsoPHSsuMaYGmWENw/w:1800/cb:1/aHR0cHM6Ly9naXRodWIuY29tL1BhcnNlRm9yZ2UvYXBpZnktYXNzZXRzL2Jsb2IvYWQzNWNjYzEzZGRkMDY4YjlkNmNiYTMzZjMyMzk2MmUzOWFlZDViMi9iYW5uZXIuanBnP3Jhdz10cnVl.webp)

# 📊 ImportYeti Scraper

> 🕒 **Last updated:** 2026-05-05

Unlock US import and export trade intelligence with ImportYeti. This scraper automates collection of supplier profiles, shipment history, and company trade data without coding. Perfect for importers seeking to identify suppliers, exporters analyzing market competition, and researchers monitoring trade patterns. Get complete customs intelligence to find new suppliers, benchmark competitor shipments, and download trade data in CSV format instantly.

> **The ImportYeti Scraper collects comprehensive supplier and company trade data, up to 50+ fields including shipment history, location details, and trading partners, with residential proxy support for reliable data extraction.**

## ✨ What Does It Do

- 📍 **Company Title** - Identify the exact name and legal entity of suppliers or trading companies
- 🚢 **Total Shipments** - Track the volume of shipments to assess company trading frequency and reliability
- 📅 **Most Recent Shipment** - Monitor current activity levels to find active traders and recent business partners
- 🌍 **Import and Export Countries** - Discover which markets companies serve and their geographic reach
- 👥 **Top Suppliers and Customers** - Identify key trading partners to understand supply chain relationships
- 💼 **Business Type and Industry** - Classify companies by sector to find relevant industry competitors
- 📝 **Product List** - Extract what companies import or export to match with your sourcing needs
- 🔗 **Contact Information** - Collect phone, email, website, and address for outreach and verification
- 📊 **HS Codes** - Track harmonized system codes to monitor specific product categories in trade flows
- 💰 **Estimated Shipping Spend** - Estimate company trading volume based on freight and shipping costs

## 🔧 Input

- **Search Query** - Enter a search term to find suppliers or companies (e.g., "aluminum", "textiles", "electronics")
- **Type** - Filter results by supplier or company type to narrow your search
- **Location** - Specify a location (e.g., "California", "New York") to find regional traders
- **Most Recent Shipment** - Filter by shipment recency (e.g., "6mo", "1y", "2y") to find active traders
- **Shipments Total** - Set a minimum shipment count to focus on high-volume trading partners
- **Industry** - Filter by industry ID to target specific sectors
- **Max Items** - Choose how many results to collect (up to 10 for free accounts, up to 1,000,000 for paid)

Example input:

```
{
  "q": "electronics",
  "type": "supplier",
  "location": "california",
  "maxItems": 50
}
```

## 📊 Output

Each supplier includes up to 50 data fields. Download as JSON, CSV, or Excel.

| 📍 Company Title | 🚢 Total Shipments | 📅 Most Recent Shipment |
| --- | --- | --- |
| 🌍 Country Code | 📍 Address | 👥 Top Suppliers |
| 👥 Top Customers | 🌍 Import Countries | 🌍 Export Countries |
| 💼 Business Type | 📝 Primary Industry | 📊 Company Size |
| 💰 Est. Shipping Spend | 📊 Revenue | 🔗 Website |
| 📞 Phone | 📧 Email | 📍 City |
| 📍 State | 📮 Postal Code | 📅 Year Established |
| 👨 Key Personnel | 📜 Certifications | 🏭 Main Products |
| 📦 HS Codes | 🚚 Avg TEU per Shipment | 📊 Avg TEU per Month |
| 📄 Registration Number | 🏛 Tax ID | 🔗 Trade Names |
| 📊 Coverage | 📅 Data Start Date | 📅 Data End Date |
| 🔗 Detail URL | ⏰ Scraped At | ❌ Error Messages |

## 💎 Why Choose the ImportYeti Scraper?

| Feature | Our Actor | Similar Scrapers |
| --- | --- | --- |
| Filter by location (US regions) | ✔️ | ❌ |
| Filter by shipment frequency | ✔️ | ❌ |
| Filter by industry ID | ✔️ | ❌ |
| Collect up to 1,000,000 results | ✔️ | Partial |
| Extract 50+ trade data fields | ✔️ | Partial |
| Top suppliers and customers lists | ✔️ | ❌ |
| Shipment history and TEU metrics | ✔️ | ❌ |
| Estimated shipping spend | ✔️ | ❌ |
| Search by company name or keyword | ✔️ | ✔️ |
| Export to CSV, JSON, or Excel | ✔️ | ✔️ |

## 📋 How to Use

No technical skills required. Follow these simple steps:

1. **Sign Up**: [Create a free account](https://console.apify.com/sign-up?fpr=vmoqkp)
2. **Find the Tool**: Search for "ImportYeti Scraper" in the Apify Store and configure your input
3. **Run It**: Click "Start" and watch your results appear

That's it. No coding, no setup, no complicated configuration. Now you can export your data in CSV, Excel, or JSON format.

## 🎯 Business Use Cases

- 📊 **Sourcing Manager** - Search for aluminum suppliers in California and filter by minimum 50 shipments to build a qualified supplier list for manufacturing RFQ
- 💼 **Export Sales Manager** - Monitor competitors' export patterns to Europe and Asia by tracking their top customers and HS codes to adjust strategy before the quarter ends
- 🔬 **Market Researcher** - Analyze top 500 electronics importers and their estimated shipping spend to forecast market growth and identify consolidation trends in the supply chain

## 🤖 Ask an AI assistant about this scraper

Open a ready-to-send prompt about this ParseForge actor in the AI of your choice:

- 💬 [**ChatGPT**](https://chat.openai.com/?q=How%20do%20I%20use%20the%20ImportYeti%20Scraper%20by%20ParseForge%20on%20Apify%3F%20Show%20me%20input%20examples%2C%20output%20fields%2C%20common%20use%20cases%2C%20and%20how%20to%20integrate%20it%20into%20a%20workflow.)
- 🧠 [**Claude**](https://claude.ai/new?q=How%20do%20I%20use%20the%20ImportYeti%20Scraper%20by%20ParseForge%20on%20Apify%3F%20Show%20me%20input%20examples%2C%20output%20fields%2C%20common%20use%20cases%2C%20and%20how%20to%20integrate%20it%20into%20a%20workflow.)
- 🔍 [**Perplexity**](https://perplexity.ai/search?q=How%20do%20I%20use%20the%20ImportYeti%20Scraper%20by%20ParseForge%20on%20Apify%3F%20Show%20me%20input%20examples%2C%20output%20fields%2C%20common%20use%20cases%2C%20and%20how%20to%20integrate%20it%20into%20a%20workflow.)
- 🅒 [**Copilot**](https://copilot.microsoft.com/?q=How%20do%20I%20use%20the%20ImportYeti%20Scraper%20by%20ParseForge%20on%20Apify%3F%20Show%20me%20input%20examples%2C%20output%20fields%2C%20common%20use%20cases%2C%20and%20how%20to%20integrate%20it%20into%20a%20workflow.)

---

## ❓ Frequently Asked Questions

**🔍 How does it work?**

The scraper sends your search query to ImportYeti, collects supplier profiles from the search results, and fetches detailed company information including shipment history, contact details, and trading partners.

**📊 How accurate is the data?**

ImportYeti sources data from US customs records and public business databases. Data accuracy depends on ImportYeti's coverage and the completeness of customs declarations filed by importers and exporters.

**📅 Can I schedule automatic runs?**

Yes. Use the Apify scheduler to run the scraper on a daily, weekly, or monthly basis to monitor new suppliers or track changes in competitor trade activity.

**⚖️ Is web scraping allowed?**

Yes, this scraper collects data from public sources. ImportYeti data is based on publicly filed US customs records. You are responsible for complying with ImportYeti's terms of service and local data regulations.

**🛡️ Will ImportYeti block me?**

ImportYeti may detect automated requests. We recommend using residential proxies to avoid rate limits and blocking.

**⚡ How long does a run take?**

Speed depends on your search results and max items. Collecting 100 results typically takes 2-5 minutes. Larger collections (1,000+ items) may take 15-60 minutes.

**⚠️ Are there any limits?**

Free accounts can collect up to 10 results per run. Paid users can collect up to 1,000,000 results per run.

## 🔗 Integrate ImportYeti Scraper with any app

- [Make](https://docs.apify.com/platform/integrations/make) - Automate workflows
- [Zapier](https://docs.apify.com/platform/integrations/zapier) - Connect 5000+ apps
- [GitHub](https://docs.apify.com/platform/integrations/github) - Version control integration
- [Slack](https://docs.apify.com/platform/integrations/slack) - Get notifications
- [Airbyte](https://docs.apify.com/platform/integrations/airbyte) - Data pipelines
- [Google Drive](https://docs.apify.com/platform/integrations/drive) - Export to spreadsheets

## 🔌 Integrate with any app

ImportYeti Scraper connects to any cloud service via [Apify integrations](https://apify.com/integrations):

- [**Make**](https://docs.apify.com/platform/integrations/make) - Automate multi-step workflows
- [**Zapier**](https://docs.apify.com/platform/integrations/zapier) - Connect with 5,000+ apps
- [**Slack**](https://docs.apify.com/platform/integrations/slack) - Get run notifications in your channels
- [**Airbyte**](https://docs.apify.com/platform/integrations/airbyte) - Pipe results into your warehouse
- [**GitHub**](https://docs.apify.com/platform/integrations/github) - Trigger runs from commits and releases
- [**Google Drive**](https://docs.apify.com/platform/integrations/drive) - Export datasets straight to Sheets

You can also use webhooks to trigger downstream actions when a run finishes. Push fresh data into your product backend, or alert your team in Slack.

---

## 💡 More ParseForge Actors

- [Etsy Scraper](https://apify.com/parseforge/etsy-scraper) - Extract product listings, prices, and seller information from Etsy
- [Trade Me Property Scraper](https://apify.com/parseforge/trade-me-property-scraper) - Collect property listings and real estate data from Trade Me
- [Rightmove Property Scraper](https://apify.com/parseforge/rightmove-property-scraper) - Gather UK property data from Rightmove
- [Indeed Scraper](https://apify.com/parseforge/indeed-scraper) - Collect job listings and employment data from Indeed
- [Redfin Scraper](https://apify.com/parseforge/redfin-scraper) - Extract US real estate and home valuation data from Redfin

Browse our complete collection of [data extraction tools](https://apify.com/parseforge) for more.

## 🚀 Ready to Start?

[Create a free account](https://console.apify.com/sign-up?fpr=vmoqkp) and collect your first 10 results for free. No coding, no setup.

## 🆘 Need Help?

- Check the FAQ section above for common questions
- Visit the [Apify support page](https://docs.apify.com) for documentation and tutorials
- Contact us to request a new scraper, propose a custom project, or report an issue at [Tally contact form](https://tally.so/r/BzdKgA)

## ⚠️ Disclaimer

> This Actor is an independent tool and is not affiliated with, endorsed by, or sponsored by ImportYeti or any of its subsidiaries. All trademarks mentioned are the property of their respective owners.

---

## ✨ Why choose this Actor

|  | Capability |
| --- | --- |
| 🎯 | **Built for the job.** Scoped specifically to this data source so you skip the parser engineering entirely. |
| 🔖 | **Structured output.** Clean, typed fields ready for analysis, dashboards, or downstream pipelines. |
| ⚡ | **Fast.** Optimized request patterns return results in seconds, not minutes. |
| 🔁 | **Always fresh.** Every run pulls live data, so the dataset reflects the source as of run time. |
| 🌐 | **No infra to manage.** Apify handles proxies, retries, scaling, scheduling, and storage. |
| 🛡️ | **Reliable.** Battle-tested across many runs and edge cases, with graceful error handling. |
| 🚫 | **No code required.** Configure in the UI, run from CLI, schedule via cron, or call from any language with the Apify SDK. |

> 📊 Production-grade structured data without the engineering overhead of building and maintaining your own scraper.

---

## 📈 How it compares to alternatives

| Approach | Cost | Coverage | Refresh | Filters | Setup |
| --- | --- | --- | --- | --- | --- |
| **⭐ ImportYeti Scraper** *(this Actor)* | $5 free credit, then pay-per-use | Full source coverage | **Live per run** | Source-native filters supported | ⚡ 2 min |
| Build your own scraper | Engineering hours | Full once built | Whenever you maintain it | Custom code | 🐢 Days to weeks |
| Paid managed APIs | $$$ monthly | Vendor-defined | Live | Vendor-defined | ⏳ Hours |
| Third-party data dumps | Varies | Subset, often stale | Periodic | None | 🕒 Variable |

Pick this Actor when you want broad coverage, server-side filtering, and no pipeline maintenance.

---

## 🚀 How to use

1. 📝 **Sign up.** [Create a free account with $5 credit](https://console.apify.com/sign-up?fpr=vmoqkp) (takes 2 minutes).
2. 🌐 **Open the Actor.** Go to the ImportYeti Scraper page on the Apify Store.
3. 🎯 **Set input.** Configure the input fields in the form (or paste a JSON), then set `maxItems`.
4. 🚀 **Run it.** Click **Start** and let the Actor collect your data.
5. 📥 **Download.** Grab your results in the **Dataset** tab as CSV, Excel, JSON, or XML.

> ⏱️ Total time from signup to downloaded dataset: **3-5 minutes.** No coding required.

---

## 💼 Business use cases

| ### 📊 Data & Analytics     - Build trend reports and dashboards from live source data - Feed BI tools, warehouses, and ML pipelines with structured records - Run periodic snapshots to track changes over time - Compare segments, regions, or categories with consistent fields | ### 🏢 Operations & Strategy     - Monitor competitor moves, pricing, and inventory shifts - Build internal directories and lookup tools backed by current data - Power workflows that depend on fresh source records - Cut manual data-gathering time from hours to minutes |
| --- | --- |
| ### 🎯 Marketing & Growth     - Identify market opportunities and trending topics - Research target audiences and customer personas at scale - Power lead-generation pipelines with verified records - Track sentiment, reviews, or social signals over time | ### 🛠️ Engineering & Product     - Prototype features that need real-world data without owning a crawler - Replace fragile in-house scrapers with a managed Actor - Wire datasets into your apps via the Apify API or webhooks - Skip the proxy, retry, and parsing maintenance entirely |

---

## 🌟 Beyond business use cases

Data like this powers more than commercial workflows. The same structured records support research, education, civic projects, and personal initiatives.

| ### 🎓 Research and academia     - Empirical datasets for papers, thesis work, and coursework - Longitudinal studies tracking changes across snapshots - Reproducible research with cited, versioned data pulls - Classroom exercises on data analysis and ethical scraping | ### 🎨 Personal and creative     - Side projects, portfolio demos, and indie app launches - Data visualizations, dashboards, and infographics - Content research for bloggers, YouTubers, and podcasters - Hobbyist collections and personal trackers |
| --- | --- |
| ### 🤝 Non-profit and civic     - Transparency reporting and accountability projects - Advocacy campaigns backed by public-interest data - Community-run databases for local issues - Investigative journalism on public records | ### 🧪 Experimentation     - Prototype AI and machine-learning pipelines with real data - Validate product-market hypotheses before engineering spend - Train small domain-specific models on niche corpora - Test dashboard concepts with live input |

---

## 🔗 Recommended Actors

- [**🔍 Google Search Scraper**](https://apify.com/parseforge/google-search-scraper) - Multi-engine SERP results with country and language targeting
- [**🗺️ Nominatim OSM Scraper**](https://apify.com/parseforge/nominatim-osm-scraper) - Geocode addresses via OpenStreetMap
- [**📊 Indexmundi Scraper**](https://apify.com/parseforge/indexmundi-scraper) - Global demographic and economic indicators
- [**📰 RAG Web Browser**](https://apify.com/parseforge/rag-web-browser) - Crawl and extract clean text from any URL for AI retrieval
- [**🌐 Website Content Crawler**](https://apify.com/parseforge/website-content-crawler) - Crawl entire sites and export structured content

> 💡 **Pro Tip:** browse the complete [ParseForge collection](https://apify.com/parseforge) for more reference-data scrapers.