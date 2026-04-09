# Craigslist Scraper

> Extract classified ads, job postings, housing listings, and for-sale items from Craigslist

[![Try on Apify](https://img.shields.io/badge/Try_on-Apify_Store-00C853?style=for-the-badge)](https://apify.com/thirdwatch)
[![Website](https://img.shields.io/badge/Website-thirdwatch.dev-000?style=for-the-badge)](https://thirdwatch.dev)

## What it does

Scrapes Craigslist classified ads across all categories including jobs, housing, for sale, services, and gigs. Extracts titles, prices, descriptions, locations, images, and posting dates. Supports all US cities and international Craigslist sites.

## Output fields

| Field | Type | Description |
|-------|------|-------------|
| title | String | Listing title |
| price | Number | Listed price |
| currency | String | Currency code |
| location | String | Neighborhood or area |
| description | String | Full listing description |
| category | String | Listing category |
| images | Array | Image URLs |
| postedDate | String | Posting date |
| attributes | Object | Listing-specific attributes |
| url | String | Direct listing URL |

## Input parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| queries | Array | Search keywords |
| city | String | Craigslist city (e.g., "sfbay", "newyork") |
| category | String | Category filter (jobs, housing, forsale) |
| maxResults | Number | Maximum results per query |
| minPrice | Number | Minimum price filter |
| maxPrice | Number | Maximum price filter |

## Example output

```json
{
  "title": "2BR Apartment in Mission District",
  "price": 2800,
  "currency": "USD",
  "location": "Mission District, SF",
  "description": "Sunny 2-bedroom apartment with hardwood floors...",
  "category": "Apartments / Housing For Rent",
  "images": ["https://images.craigslist.org/..."],
  "postedDate": "2026-04-08",
  "attributes": {
    "bedrooms": 2,
    "bathrooms": 1,
    "sqft": 850,
    "laundry": "in-unit"
  },
  "url": "https://sfbay.craigslist.org/sfc/apa/..."
}
```

## Pricing

| Plan | Price |
|------|-------|
| Pay per result | $0.001/result |
| Free tier | Available on Apify |

## Use cases

- Real estate market analysis and rental price tracking
- Used goods price monitoring and deal finding
- Local job market research across US cities
- Market research for local services demand
- Academic research on classified ad trends

## Getting started

1. Go to the [Apify Store](https://apify.com/thirdwatch)
2. Find the **Craigslist Scraper**
3. Select city, category, and enter search terms
4. Run and download results as JSON, CSV, or Excel

## Related scrapers by Thirdwatch

- [Google Maps Scraper](https://github.com/thirdwatch-dev/google-maps-scraper) -- Business listings
- [Indeed Scraper](https://github.com/thirdwatch-dev/indeed-scraper) -- Job listings
- [Amazon Scraper](https://github.com/thirdwatch-dev/amazon-scraper) -- Product data
- [Trustpilot Scraper](https://github.com/thirdwatch-dev/trustpilot-scraper) -- Reviews
- [Flipkart Scraper](https://github.com/thirdwatch-dev/flipkart-scraper) -- E-commerce data

## About Thirdwatch

[Thirdwatch](https://thirdwatch.dev) builds production-ready web scraping APIs. 18 scrapers for jobs, e-commerce, reviews, social media, and business data.

## License

MIT
