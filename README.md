# Business Insights 360 – Dashboard Walkthrough

A view-by-view walkthrough of the Power BI dashboard, with a screenshot followed by a description of what it shows.

---

## 1. Home

![Home](screenshots/home.png)

The landing page of the dashboard. It provides navigation tiles into each of the six functional views:

- **Info** – Download the user manual and key information about the tool.
- **Finance View** – P&L statement for any customer/product/country, aggregated over any time period.
- **Sales View** – Customer/product performance over key metrics (Net Sales, Gross Margin) with a profitability/growth matrix.
- **Marketing View** – Product performance over key metrics with the same profitability/growth matrix, sliced by market.
- **Supply Chain View** – Forecast Accuracy, Net Error, and risk profile by product, segment, category, and customer.
- **Executive View** – A top-level dashboard consolidating insights across all business dimensions for executives.
- **Support** – Contact point to get issues resolved by a support specialist.

The footer shows the report refresh date, currency/units used (Millions & Dollar), and the data load cutoff (Sales data loaded until Dec 21).

---

## 2. Finance View

![Finance View](screenshots/finance-view.png)

Focused on the company's financial performance and P&L breakdown.

- **KPI cards**: Net Sales ($3.74bn), Gross Margin % (38.08%), Net Profit % (-13.98%) — each shown against a Benchmark (BM) with variance.
- **P&L Statement table**: Full waterfall from Gross Sales → Pre-Invoice Deduction → Net Invoice Sales → Post Discounts/Deductions → Net Sales → COGS (Manufacturing, Freight, Other) → Gross Margin → Operating Expenses → Net Profit, each with BM and % change columns.
- **Net Sales trend chart**: Monthly Actuals vs Benchmark from Sep 2021 to Aug 2022, highlighting seasonality (peak around Nov–Dec 2021).
- **Region table**: Net Sales and % change by region (APAC, LATAM, NA, EU).
- **Segment table**: Net Sales and % change by product segment (Accessories, Desktop, Networking, Notebook, Peripherals, Storage).
- Global slicers for Region/Market, Customer, and Segment/Category, plus Year and Quarter/YTD/YTG toggles apply across the whole page.

---

## 3. Sales View

![Sales View](screenshots/sales-view.png)

A deep dive into sales performance at the customer and product level.

- **Customer Performance table**: Net Sales $, Gross Margin $, and Gross Margin % for every customer (e.g., Amazon at $496.9M net sales / 36.8% GM, AtliQ Exclusive at 46.0% GM).
- **Product Performance table**: Same metrics broken down by segment (Notebook is the largest at $1,580.4M net sales).
- **Unit Economics donut charts**: P&L values by description — Net Sales vs Post Invoice Deductions vs Pre-Invoice Deductions, and COGS vs Gross Margin, shown as proportions of the total.
- **Performance Matrix (bubble chart)**: Gross Margin % vs Net Sales $ by country/region, color-coded by region (APAC, EU, LATAM, NA) — used to spot high-value, high-margin markets (e.g., USA and India stand out on net sales; Australia/China lead on margin).

---

## 4. Market View

![Market View](screenshots/market-view.png)

Product-category and market-level profitability analysis.

- **Product Performance table**: Net Sales $, Gross Margin $/%, and Net Profit $/% by category (e.g., Business Laptop $765.2M net sales but -13.8% net profit margin; every category is currently net-loss making).
- **Performance Matrix (bubble chart)**: Gross Margin % vs Net Sales $, bubbles sized and colored by division (N&S, P&A, PC) — shows which product lines drive volume vs margin.
- **Region/Market/Customer performance donut**: Total COGS vs Gross Margin as a share of Net Sales.
- **Waterfall chart**: Bridges from Gross Margin → Operating Expenses → Net Profit $, visually showing how operating expenses erode margin into a net loss.
- A **"Show NP %"** toggle lets the user switch between absolute and percentage net profit views.

---

## 5. Supply Chain View

![Supply Chain View](screenshots/supply-chain-view.png)

Forecasting accuracy and risk monitoring across customers and products.

- **KPI cards**: Forecast Accuracy (81.2%, up +1.2 pts vs LY), Net Error (-3,472.69K), Absolute Error (6,899.04K).
- **Accuracy / Net Error Trend chart**: Monthly Net Error (bars) plotted against Forecast Accuracy % (current year vs LY line), showing accuracy dipped notably around July–September.
- **Key Metrics by Customer table**: Forecast Accuracy %, Net Error %, and a Risk flag (OOS = Out of Stock, ES = Excess Stock) per customer — most customers are flagged OOS, indicating a tendency toward under-forecasting/stockouts.
- **Key Metrics by Products table**: Same metrics by segment — Peripherals and Storage have the weakest forecast accuracy (68.2% and 71.5%) and largest negative net error, marking them highest risk.

---

## 6. Executive View

![Executive View](screenshots/executive-view.png)

The consolidated, top-level view for leadership — combines Finance, Sales, Market, and Supply Chain metrics on one page.

- **KPI cards**: Net Sales ($3.74bn), Gross Margin % (38.08%), Net Profit % (-13.98%), Forecast Accuracy (81.2%) — each with BM/LY/Target comparisons.
- **Revenue by Division donut**: Split across PC, P&A, and N&S divisions (PC leads at 61.33%).
- **Revenue by Channel donut**: Retailer (72.97%), Direct (16.36%), Distributor (10.67%).
- **Key Insights by Sub Zone table**: Net Sales, Gross Margin %, Net Profit %, Net Error %, AtliQ Market Share %, and Risk flag for each sub-zone (ANZ, India, LATAM, NA, NE, ROA, SE) — used to spot underperforming or high-risk regions at a glance.
- **PC Market Share Trend (stream/area chart)**: AtliQ's share vs competitors (bp, dale, innovo, others, pacer) from 2018 to 2022 Est — AtliQ's share has declined from 46.6% to 46.4%, with a dip to ~52% mid-period.
- **Yearly trend chart**: Net Sales, Gross Margin %, Net Profit %, and AtliQ Market Share % together over 2018–2022 Est.
- **Top 5 Customers / Top 5 Products tables**: Ranked by Net Sales $, with RC % (revenue contribution) and GM %.

---

*BM = Benchmark, LY = Last Year, OOS = Out of Stock, ES = Excess Stock, EI = Excess Inventory. Values are in Millions ($) unless noted otherwise.*
