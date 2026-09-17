
---

## 🧹 Data Cleaning & Preparation

Based on the structure of the dashboards, the following preparation steps were applied to the underlying monthly financial data:

- Standardized monthly time-series data (Jan–Dec) across revenue, gross profit, and EBITDA figures
- Organized data by consistent business dimensions: **Business Unit**, **Region**, and **Product Category**
- Structured budget and forecast figures alongside actuals to enable direct comparison
- Prepared aggregation-ready fields for revenue rollups by business unit, region, and product category
- Ensured consistent formatting (currency in $M, percentages) to support clean KPI card and chart rendering

---

## ⚙️ Feature Engineering / Data Modeling

### Calculated Metrics

- **Gross Profit** = Revenue − Cost of Goods Sold
- **Gross Margin %** = Gross Profit ÷ Total Revenue
- **EBITDA** and **EBITDA Margin %**
- **Revenue Growth %** (YoY)
- **Average Selling Price (ASP)** = Revenue ÷ Units Sold
- **Variance Amount** = Actual − Budget
- **Variance %** = Variance Amount ÷ Budget
- **Forecast Variance %** = (Actual − Forecast) ÷ Forecast
- **Net Cash Flow**

### Data Model

The workbook organizes data along three primary analytical dimensions — **Business Unit** (Cloud Services, Cybersecurity, Data & Analytics, Enterprise Solutions), **Region** (North America, Europe, Asia Pacific, Middle East & Africa), and **Product Category** (Analytics, Cloud, Cybersecurity, Enterprise Software) — with a monthly time dimension (Jan–Dec) used across trend charts. Budget and forecast figures are maintained as parallel fields to actual revenue for variance calculations. The workbook does not present a formal star-schema data model in the screenshots provided; metrics are aggregated directly through Excel pivot tables and charts.

---

## 📊 Business KPIs

| KPI | Description |
|---|---|
| Total Revenue | Overall revenue generated across all business units for FY 2024–2025 |
| Gross Profit | Revenue remaining after direct costs |
| Gross Margin % | Gross profit as a percentage of revenue |
| EBITDA | Earnings before interest, tax, depreciation, and amortization |
| EBITDA Margin % | EBITDA as a percentage of revenue |
| Total OPEX | Total operating expenses |
| Net Cash Flow | Net cash generated after operating activities |
| Revenue Growth % | Year-over-year revenue growth rate |
| Units Sold | Total volume of units sold |
| ASP (Average Selling Price) | Average revenue per unit sold |
| Budget / Actual / Forecast | Planned vs. realized vs. projected revenue |
| Variance % / Forecast Variance % | Deviation of actuals from budget and forecast |

---

## 📈 Dashboard Overview

### Dashboard 1 — Executive Financial Dashboard

**Purpose:** Provides a high-level executive summary of corporate financial health for FY 2024–2025.

Components:
- KPI cards: Total Revenue ($2,166.4M), Gross Profit ($1,229.0M), Gross Margin (56.73%), EBITDA ($490.9M), EBITDA Margin (22.66%), Total OPEX ($738.0M), Net Cash Flow ($381.7M), Revenue Growth (16.99%)
- **Revenue & Profitability Trend** — monthly line chart of Total Revenue vs. Gross Profit (Jan–Dec)
- **Profitability By Region** — donut chart of gross profit contribution by region
- **Revenue By Business Unit** — 3D column chart comparing revenue across the four business units
- **Revenue VS EBITDA** — monthly line chart comparing total revenue against EBITDA

This dashboard gives leadership a single-view snapshot of top-line growth, profitability, and cash position.

### Dashboard 2 — Revenue & Profitability Analysis

**Purpose:** Drills into the drivers behind revenue growth and profitability at the product and business-unit level.

Components:
- KPI cards: Total Revenue, Revenue Growth, Units Sold (136.8K), ASP ($15.8K), Gross Profit, Gross Margin, EBITDA, EBITDA Margin
- **Revenue & Profitability Trend** — same monthly trend as Dashboard 1
- **Revenue By Product Category** — donut chart across Analytics, Cloud, Cybersecurity, Enterprise Software
- **Revenue By Business Unit** — horizontal bar chart of revenue by business unit
- **Gross Margin By Product Category** — 3D column chart comparing margin % across product categories
- **Top 10 Products By Revenue** — horizontal bar chart ranking individual products (e.g., Cloud Infrastructure, Network Security, Enterprise ERP Suite)

This dashboard supports product-mix and profitability-driver analysis for revenue optimization decisions.

### Dashboard 3 — Budget VS Actual Performance

**Purpose:** Tracks budget adherence and forecast accuracy across the fiscal year.

Components:
- KPI cards: Budget ($3,137.8M), Actual ($2,166.4M), Variance Amount (-$971.5M), Variance % (-30.96%), Forecast ($3,328.6M), Forecast Variance % (-34.92%)
- **Budget VS Actual Revenue Trend** — monthly bar chart comparing budgeted vs. actual revenue
- **Budget VS Actual by Business Unit** — bar chart comparing budget vs. actual revenue per business unit
- **Budget VS Actual By Region** — bar chart comparing budget vs. actual revenue per region
- **Variance By Budget Category** — bar chart of variance figures by region
- **Forecast VS Actual** — comparison of full-year forecast against actual revenue with variance %

This dashboard enables finance teams to assess forecast accuracy and identify where actuals deviated most from plan.

---

## 💡 Key Insights

- Total revenue for FY 2024–2025 reached **$2,166.4M**, representing **16.99% revenue growth**, with EBITDA of **$490.9M** at a **22.66% EBITDA margin**.
- **Cloud Services** was the top-performing business unit at **$596.0M** in revenue, followed by Data & Analytics ($578.3M), Enterprise Solutions ($527.6M), and Cybersecurity ($464.4M).
- **Europe** was the most profitable region, contributing **$486.7M** in gross profit, ahead of North America ($340.2M), Asia Pacific ($279.2M), and Middle East & Africa ($122.9M).
- **Cybersecurity** carried the highest gross margin among product categories at **59.27%**, followed closely by Analytics (58.95%), while Cloud (54.58%) and Enterprise Software (54.50%) trailed.
- **Cloud Infrastructure** was the top individual product by revenue at **$218.3M**, followed by Network Security ($207.3M) and Enterprise ERP Suite ($188.7M).
- Actual revenue of **$2,166.4M** came in **$971.5M below the $3,137.8M budget**, a shortfall of **-30.96%**.
- Every business unit fell short of its revenue budget, with **Data & Analytics** showing the largest gap between budgeted ($855.9M) and actual ($578.3M) revenue.
- Full-year forecast projected **$3,328.6M** in revenue, resulting in a **-34.92% forecast variance** against actual results.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Microsoft Excel | Dashboard development and layout |
| Pivot Tables | Aggregating revenue, profit, and budget data |
| Pivot Charts | Trend, comparison, and distribution visualizations |
| Excel Formulas | KPI and margin/variance calculations |

---

## 📁 Project Structure
