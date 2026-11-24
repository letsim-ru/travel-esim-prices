# How much mobile internet costs while travelling — travel eSIM prices in 196 countries

**Сколько стоит мобильный интернет в поездке: цены туристических eSIM по 196 странам**

Open dataset by [Letsim](https://letsim.ru) (letsim.ru).

**Disclosure:** conducted by Letsim, a commercial travel eSIM provider that sells the plans discussed here. Data, rules and raw inputs are published so that the results can be checked independently.

Page with findings and methodology (in Russian): https://letsim.ru/issledovaniya/stoimost-interneta-v-poezdke

## What is inside

Final retail prices of Letsim travel eSIM plans in Russian roubles for 196 destinations, prices as of 23 November 2026:

- minimum price, 1 GB / 7 days, 10 GB / 30 days, price per GB of the 10 GB pack;
- unlimited "Lite" for 7 days (daily full-speed cap, reduced speed after it);
- the cheapest regional plan (10 GB / 30 days) that covers the destination, when it is cheaper than the country plan.

Key findings:

- median price of 10 GB / 30 days across 192 destinations — 2,465 RUB;
- the cheapest is Turkey (590 RUB), the most expensive New Caledonia (28,690 RUB) — a 49× difference;
- by part of the world the median is lowest in Europe (1,040 RUB) and highest in Africa (5,890 RUB);
- in 17 destinations a regional plan is cheaper than the country plan for the same 10 GB / 30 days.

These are prices of one store, not market averages. They follow supplier costs and are updated together with the price list.

## Files

| File | Rows | Description |
|---|---|---|
| `data.csv` | 196 | One row per destination. UTF-8 with BOM, `;` separator, prices in RUB |
| `data.json` | 196 | Same data in JSON with metadata |
| `notebook.ipynb` | — | Example notebook: median, cheapest and most expensive destinations, medians by part of the world, cheaper regional plans |

### Columns (`data.csv`)

| Column | Meaning |
|---|---|
| `country_code` | ISO 3166-1 alpha-2 code |
| `country_ru` | Destination name in Russian |
| `world_region` | Part of the world (Russian) |
| `min_price_rub` | Cheapest plan for the destination |
| `price_1gb_7d_rub` | 1 GB for 7 days |
| `price_10gb_30d_rub` | 10 GB for 30 days |
| `price_per_gb_10gb_rub` | Price per GB of the 10 GB / 30 days pack |
| `unlimited_lite_7d_rub` | Unlimited "Lite" for 7 days |
| `cheaper_regional_plan` | Cheapest covering regional plan, if cheaper than the country plan |
| `cheaper_regional_10gb_30d_rub` | Its price for 10 GB / 30 days |
| `plans_count` | Number of plan × duration options for the destination |
| `page_url` | Destination page on letsim.ru |

Empty cell — no such plan for the destination.

## Versions

Release v1 — 24 November 2026. Frozen copies on the website: `https://letsim.ru/issledovaniya/stoimost-interneta-v-poezdke/v1-2026-11-24/` (`data.csv`, `data.json`). Files at the page root are updated with new data; archived versions with a DOI are on Zenodo.

## License and citation

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

Cite as: *Letsim (letsim.ru). How much mobile internet costs while travelling: travel eSIM prices in 196 countries. Prices as of 23 November 2026.*
