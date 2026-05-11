
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


---



## Files

| File | Description |
|------|-------------|
| `sample-chocolate-shipments-data-all-Apr-2025.xlsx` | Source data workbook with shipments, dimension tables, and a calendar table |
| `chocolate_powerbi.pbix` | Power BI Desktop report file for interactive data visualization |

---

## Data Model

The Excel workbook contains three sheets that form a star schema:

### `Shipments` (Fact Table)
The core transactional table with 25,076 rows.

| Column | Type | Description |
|--------|------|-------------|
| `ShipmentID` | Text | Unique identifier for each shipment (e.g., `S00000004`) |
| `SPID` | Text | Salesperson ID — foreign key to Dimension Data |
| `PID` | Text | Product ID — foreign key to Dimension Data |
| `GID` | Text | Geography ID — foreign key to Dimension Data |
| `Shipdate` | Date | Date the shipment was dispatched |
| `Amount` | Number | Revenue value of the shipment (currency) |
| `Boxes` | Integer | Number of boxes shipped |
| `Order_Status` | Text | Status of the order: `Delivered`, `Shipped`, `Placed`, or `Cancelled` |

**Date range:** 2 Jan 2023 – 31 Mar 2025

**Order statuses:**
- `Delivered` — shipment completed
- `Shipped` — in transit
- `Placed` — order received, not yet dispatched
- `Cancelled` — order cancelled

---

### `Dimension Data` (Dimension Table)
Contains three embedded lookup tables in a single sheet:

**Products** (22 unique products)

| Column | Description |
|--------|-------------|
| `PID` | Product ID |
| `Product` | Product name (e.g., Milk Bars, Eclairs, Almond Choco) |
| `Category` | Product category: `Bars`, `Bites`, or `Other` |
| `Cost_per_box` | Cost per box in currency units |

**Geographies** (6 regions)

| Column | Description |
|--------|-------------|
| `GID` | Geography ID |
| `Geo` | Country (India, USA, Canada, New Zealand, Australia, UK) |
| `Region` | Regional grouping: `APAC`, `Americas`, or `Europe` |

**Salespeople** (25 unique salespeople)

| Column | Description |
|--------|-------------|
| `SPID` | Salesperson ID |
| `Sales_person` | Full name of the salesperson |
| `Team` | Sales team: `Yummies` or `Delish` |
| `Picture` | URL to the salesperson's profile picture |

---

### `Calendar` (Date Dimension Table)
A formula-driven date table used for time-intelligence calculations in Power BI.

| Column | Description |
|--------|-------------|
| `cal_date` | Full date |
| `Month_num` | Month number (1–12) |
| `month_name` | Month name (e.g., January) |
| `year` | Year |
| `weekday_num` | Weekday number (1 = Monday) |
| `weekday_name` | Weekday name (e.g., Monday) |

---


## Quick Stats

| Metric | Value |
|--------|-------|
| Total shipment records | 25,076 |
| Date range | Jan 2023 – Mar 2025 |
| Unique salespeople | 25 |
| Unique products | 22 |
| Geographies | 6 countries, 3 regions |
| Sales teams | 2 (Yummies, Delish) |
| Order statuses | 4 (Delivered, Shipped, Placed, Cancelled) |
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

> *![Dashboard](/Dashboard.png)*

---

## ⚙️ How to Use

1. Download the `chocolate_powerbi.pbix` file
2. Open in **Power BI Desktop** (version 2026.04 or later recommended)
3. Go to **Home → Transform Data → Data Source Settings** and update the path to your local copy of the Excel file
4. Click **Refresh** to load the data
5. Explore the 7 report pages using slicers and cross-filters

--- 

## 📌 Conclusion
This project showcases end-to-end data analysis skills — from data cleaning to dashboard creation and insight generation.

It demonstrates my ability to solve business problems using data.

---

## 🎯 What I Learned
- Data modeling in Power BI  
- Writing efficient DAX  
- Designing user-friendly dashboards  

---

## 🤝 Connect With Me
If you found this project useful or have feedback, feel free to connect!


⭐ If you like this project, don't forget to star the repository!
