# Saudi Vision 2030 — KPI Progress Tracker

An interactive dashboard tracking Saudi Arabia's Vision 2030 transformation across 11 key performance indicators, built with real data from official government sources.

**[→ View Live Dashboard](https://yourusername.github.io/vision2030-tracker)**

---

## Overview

Saudi Vision 2030 is the Kingdom's national strategy to diversify its economy, empower its citizens, and reduce dependence on oil. Nine years into the program, 93% of KPIs have been achieved or are on track — but not all indicators tell the same story.

This project collects, cleans, and visualizes the latest data from the 2024 Annual Report and official Saudi open data platforms to present an honest, data-driven view of progress.

### Key Findings

- **8 out of 11 KPIs exceeded their targets** — including unemployment (hit 2030 target 6 years early) and female workforce participation (33.5% vs 30% target)
- **PIF assets grew 501%** from $152B to $913B since 2016
- **Non-oil exports lag significantly** at 25.2% of non-oil GDP against a 50% target
- **Environmental performance remains the weakest indicator** — Saudi Arabia ranked last (67/67) on the Climate Change Performance Index

---

## Dashboard Features

- **Real-time filtering** by pillar (Economy / Society / Governance)
- **Dual chart panels** with 6 switchable trend visualizations (Unemployment, Female Workforce, GDP, Oil vs Non-Oil Revenue, PIF Assets, Tourism)
- **Live ticker** with key stat changes since 2016
- **Animated counters** and progress bars on load
- **Fully responsive** — works on desktop, tablet, and mobile
- **Single HTML file** — no build step, no dependencies beyond a CDN-loaded Chart.js

---

## Data Sources

| Source | Data Used | URL |
|--------|-----------|-----|
| Vision 2030 Annual Report 2024 | All KPI targets, baselines, actuals | [vision2030.gov.sa](https://vision2030.gov.sa/en/annual-reports) |
| DataSaudi (GASTAT) | GDP, Unemployment, Labor Force, Government Revenue | [datasaudi.sa](https://datasaudi.sa/en) |
| PIF Annual Report 2024 | PIF Assets Under Management (yearly) | [pif.gov.sa](https://www.pif.gov.sa/en/investors/annual-reports/) |
| Saudi Ministry of Tourism | International tourist arrivals (yearly) | [sta.gov.sa](https://www.sta.gov.sa/en/open-data) |
| Housing Program Report 2024 | Homeownership rate (yearly) | [momah.gov.sa](https://momah.gov.sa) |
| Saudi Open Data Portal | Supplementary CSV datasets | [open.data.gov.sa](https://open.data.gov.sa) |
| Climate Change Performance Index | Environmental ranking | [ccpi.org](https://ccpi.org/country/sau/) |

---

## Datasets Included

The `data/` folder contains 5 CSV files downloaded from DataSaudi:

| File | Period | Description |
|------|--------|-------------|
| `Unemployment-Rate-by-Gender.csv` | Q2 2016 – Q3 2025 | Quarterly unemployment by gender |
| `Labor-Force-Participation-Rate-by-Gender.csv` | Q2 2016 – Q3 2025 | Quarterly workforce participation by gender |
| `Evolution-of-Real-Nominal-and-Seasonally-Adjusted-Real-GDP--Annual.csv` | 2010 – 2025 | Annual GDP (Real, Nominal, Seasonally Adjusted) |
| `Government-Revenues-and-Expenditures--Annual.csv` | 1969 – 2025 | Oil revenue, non-oil revenue, expenditures |
| `Operating-Revenues-and-Expenses-by-Economic-Activity.csv` | 2019 – 2024 | Private sector revenue by industry |

The Excel workbook `Vision_2030_KPI_Tracker.xlsx` contains three sheets: KPI Scorecard, Yearly Trends, and Sources.

---

## Tools & Technologies

- **HTML / CSS / JavaScript** — Single-page interactive dashboard
- **Chart.js** — Line charts, bar charts, stacked charts with target annotations
- **Excel (openpyxl)** — Structured KPI workbook with formulas
- **Python (pandas)** — Data cleaning and preprocessing
- **Power BI** — Companion dashboard (local .pbix file)
- **GitHub Pages** — Deployment

---

## Project Structure

```
vision2030-tracker/
├── index.html                              # Interactive dashboard
├── Vision_2030_KPI_Tracker.xlsx            # Excel workbook (3 sheets)
├── data/
│   ├── Unemployment-Rate-by-Gender.csv
│   ├── Labor-Force-Participation-Rate-by-Gender.csv
│   ├── Evolution-of-Real-Nominal-and-Seasonally-Adjusted-Real-GDP--Annual.csv
│   ├── Government-Revenues-and-Expenditures--Annual.csv
│   └── Operating-Revenues-and-Expenses-by-Economic-Activity.csv
└── README.md
```

---

## How to Run Locally

No build step needed. Just clone and open:

```bash
git clone https://github.com/yourusername/vision2030-tracker.git
cd vision2030-tracker
open index.html
```

Or simply download `index.html` and open it in any browser.

---

## KPI Summary Table

| KPI | 2016 | 2024 | Target | Status |
|-----|------|------|--------|--------|
| Unemployment Rate | 12.3% | 7.0% | 7.0% (2030) | ✅ Exceeded |
| Female Workforce | 17.0% | 33.5% | 30.0% (2030) | ✅ Exceeded |
| Private Sector GDP | 40.0% | 47.0% | 46.0% (2024) | ✅ Exceeded |
| PIF Assets | $152B | $913B | $2,670B (2030) | ✅ Exceeded |
| Homeownership | 47.0% | 65.4% | 70.0% (2030) | ✅ Exceeded |
| Tourist Arrivals | 18.0M | 29.7M | 70.0M (2030) | 🟡 On Track |
| Volunteers | 23K | 1.2M | 1.0M (2030) | ✅ Exceeded |
| E-Government Rank | #36 | #6 | Top 5 (2030) | ✅ Exceeded |
| E-Participation Rank | #39 | #7 | Top 10 (2030) | ✅ Exceeded |
| Non-Oil Exports % GDP | 16% | 25.2% | 50% (2030) | 🔴 Behind |
| Environmental Index | #67/67 | #67/67 | — | 🔴 Behind |

---

## Author

**Nawaf Badr Almutairi**
BSc Computer Science — Northumbria University

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/yourprofile)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?style=flat&logo=github)](https://github.com/yourusername)

---

## License

This project uses publicly available open data from Saudi government sources. All data is cited in the Sources sheet and dashboard footer. Built for educational and portfolio purposes.
