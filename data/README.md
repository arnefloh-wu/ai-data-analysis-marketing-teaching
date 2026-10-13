# Data

All datasets describe **Alpenglow**, a fictional Vienna-based premium chocolate brand sold in six European markets (AT, DE, FR, IT, NL, PL). The data are synthetic: they look and behave like real marketing data, but no real company or customer is behind them.

## `mmm/alpenglow_weekly.csv` — weekly country panel (936 rows = 6 countries × 156 weeks)

| Column | Description |
|--------|-------------|
| `week` | Monday of the ISO week, 2023-01-02 … 2025-12-22 (156 ISO weeks; 2025 holds 51 weeks) |
| `country` | ISO-2 code: AT, DE, FR, IT, NL, PL |
| `sales_units_k` | Units sold (thousands) |
| `revenue_eur_k` | Revenue (thousand EUR) = units × price |
| `price_eur` | Average realised retail price per unit (EUR) |
| `promo_share` | Share of volume sold on promotion (0–1) |
| `distribution` | Weighted distribution (share of retail outlets stocking the brand, 0–1) |
| `competitor_spend_k` | Index of competitor media spend (thousand EUR equivalent) |
| `consumer_confidence` | Consumer confidence index, de-meaned |
| `temperature_c` | Average weekly temperature (°C) |
| `xmas`, `easter`, `valentine` | Holiday dummies (pre-holiday selling weeks) |
| `spend_tv_k` | TV advertising spend (thousand EUR) |
| `spend_online_video_k` | Online video spend (thousand EUR) |
| `spend_paid_search_k` | Paid search spend (thousand EUR) |
| `spend_paid_social_k` | Paid social spend (thousand EUR) |
| `spend_ooh_k` | Out-of-home spend (thousand EUR) |

## `mmm/country_meta.csv` — country metadata

Population (millions), GDP per capita (thousand EUR), Hofstede scores (individualism, uncertainty avoidance, long-term orientation; approximate published values), Eurozone membership, years since market entry, retail concentration (share of top-3 retailers).
