#  Chocolate Shipments Sales Dashboard

A Power BI report delivering end-to-end visibility into chocolate shipment sales — tracking revenue, profitability, and team performance across global markets from 2023 to 2025.

---

## 🚀 Overview

This project focuses on analyzing chocolate shipment data across multiple geographies, product lines, and sales teams. It provides actionable insights using Power BI and DAX, helping stakeholders monitor sales trends, evaluate salesperson performance, and compare year-over-year profitability to drive smarter business decisions.

---

## 🎯 Objectives

- Analyze shipment revenue, cost, and profit across products and regions
- Identify top-performing salespeople and teams
- Track monthly and yearly sales trends
- Compare current vs. prior year performance (YoY analysis)
- Improve decision-making through interactive, drill-down dashboards

---

## 📂 Dataset

- **Source:** `sample-chocolate-shipments-data-all-Apr-2025.xlsx`
- **Size:** 25,076 rows × 8 columns
- **Date Range:** January 2023 – March 2025

**Features:**

| Column | Description |
|--------|-------------|
| `ShipmentID` | Unique identifier for each shipment |
| `SPID` | Salesperson ID |
| `PID` | Product ID |
| `GID` | Geography ID |
| `Shipdate` | Date the shipment was dispatched |
| `Amount` | Revenue value of the shipment |
| `Boxes` | Number of boxes shipped |
| `Order_Status` | Status: Delivered, Shipped, Placed, or Cancelled |

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** — dashboard development and visualization
- **Microsoft Excel** — data source and dimension tables
- **DAX** — calculated measures (profit %, YoY comparison, amount per box)
- **Power Query** — data transformation and table relationships

---

## 📊 Key Insights

- 📌 **Insight 1:** Revenue and profit vary significantly by geography — certain APAC markets outperform Americas and Europe in total amount shipped.
- 📌 **Insight 2:** The **Yummies** and **Delish** teams show distinct performance patterns across products and regions, useful for targeted coaching.
- 📌 **Insight 3:** Monthly shipment trends reveal clear seasonality, with notable peaks identifiable in the year-over-year line chart.
- 📌 **Insight 4:** A subset of salespeople generate disproportionately high profit margins, highlighted by the profit % leaderboard on Page 5.

---

## 📈 Dashboard Features

-  Interactive filters & slicers (geography, date range)
-  KPI cards (Total Amount, Total Cost, Total Profit, Profit %, Shipment Count, Total Boxes)
-  Trend analysis via monthly and yearly line charts
-  Year-over-year profit comparison
-  Salesperson performance tables and pivot breakdowns
-  Cross-filtering — clicking any visual filters the entire page
-  Drill-down by product, region, team, and salesperson
-  Executive summary page consolidating all key metrics

---

## 🧠 Business Impact

- Enables sales managers to quickly identify underperforming regions or products
- Supports data-driven target setting for individual salespeople and teams
- Reduces time spent on manual reporting with automated, refreshable dashboards
- Facilitates strategic planning through YoY trend visibility

---

## 📷 Screenshots

> **

---

## ⚙️ How to Use

1. Download the `chocolate_powerbi.pbix` file
2. Open in **Power BI Desktop** (version 2026.04 or later recommended)
3. Go to **Home → Transform Data → Data Source Settings** and update the path to your local copy of the Excel file
4. Click **Refresh** to load the data
5. Explore the 7 report pages using slicers and cross-filters

---

