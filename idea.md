# Indeed Jobs Aggregator and Alert API

## Idea
Offer an actor that aggregates Indeed job listings at scale and provides deduplicated, normalized job feeds with alerting and talent-market analytics.

## Why this is trending/sellable
- `indeed-scraper` shows paid demand (`1146` users in 30 days with paid-per-result pricing).
- Jobs data appears in multiple paid actor variants, indicating recurring purchase behavior.

## How to implement
1. Inputs: role queries, locations, salary filter, job type, remote filter.
2. Extraction: title, company, location, salary, posting age, job url.
3. Cleanup: canonicalize company names, deduplicate cross-query overlap.
4. Analytics: role trend by city, salary range distribution, and posting velocity.
5. Delivery: dataset, API-friendly JSON, and scheduled alerts.
6. Cost control: adaptive depth based on result density.

## Monetization
- `PRICE_PER_DATASET_ITEM` as default.
- Subscription tier for managed daily pipelines and historical snapshots.
