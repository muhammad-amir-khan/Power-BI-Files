# Power BI Portfolio

> A collection of Power BI dashboards and reports built to demonstrate data modelling, DAX, and business intelligence storytelling across real-world domains.

---

## About

This repository serves as my Power BI portfolio — each folder contains a self-contained project with the `.pbix` file, the underlying dataset, a dashboard screenshot, and a detailed README explaining the analysis, key metrics, and insights.

Projects span HR analytics, live API integrations, and will grow to cover finance, sales, operations, and more.

---

## Projects

| # | Project | Domain | Data Source | Key Focus |
|---|---|---|---|---|
| 01 | [HR Analytics Dashboard](./HR%20Analytics/) | Human Resources | CSV · 1,480 employees · 39 features | Attrition analysis, workforce demographics, engagement & risk scoring |
| 02 | [Pakistan Weather Dashboard](./Weather%20Dashboard/) | Weather / API Integration | OpenWeatherMap API · 20 cities · 5-day forecast | Live REST API ingestion, real-time conditions, geospatial map, forecast trends |
| 03 | [Contoso Sales Intelligence](./Contoso%20Sales%20Intelligence/) | Retail / Sales | Contoso DW · $12.4B revenue · FY07–FY09 | Multi-channel executive dashboard, Field Parameters, time intelligence, YOY analysis |

---

## Repository Structure

```
Power-BI-Files/
│
├── HR Analytics/
│   ├── HR Dashboard.pbix       ← Power BI report file
│   ├── HR_Analytics.csv        ← Raw dataset
│   ├── HR Analytics.jpeg       ← Dashboard screenshot
│   └── README.md               ← Project documentation
│
├── Weather Dashboard/
│   ├── Weather Dashboard.pbix  ← Power BI report file (live API connected)
│   ├── weather_dashboard.png   ← Dashboard screenshot
│   └── README.md               ← Project documentation
│
├── Contoso Sales Intelligence/
│   ├── Contoso Sales Intelligence.pbix  ← Power BI report file
│   ├── contoso_sales_intelligence.png   ← Dashboard screenshot
│   └── README.md                        ← Project documentation
│
└── README.md                   ← This file
```

---

## Skills Demonstrated

- **Data Modelling** — star schema design, dual fact tables, relationships, calculated columns
- **DAX** — time intelligence (SAMEPERIODLASTYEAR, ALLEXCEPT), dynamic labels with conditional color, Max/Min marker annotations, dynamic SVG icon generation, KPI calculations
- **Power Query (M)** — REST API integration, parameterised web calls, list iteration, in-query data transformation
- **Field Parameters** — dynamic metric switching (Revenue / Cost / Profit) without SWITCH logic or bookmarks
- **Report Design** — multi-section dashboards with consistent theming, interactive slicers, and conditional formatting
- **Storytelling** — translating raw data into clear, actionable insights for non-technical stakeholders

---

## Tools & Stack

| Tool | Purpose |
|---|---|
| Powe