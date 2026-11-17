# Interactive Sales Dashboard (Excel Online)

An end-to-end sales performance dashboard built entirely in Excel Online, featuring automated data cleaning, advanced PivotTable modeling, interactive slicers, and custom KPI cards.

## 📊 Dashboard Overview
* **Total Revenue:** $1.85M 
* **Total Orders:** 1,150 
* **Quantity Sold:** 5,054 
* **Average Order Value (AOV):** $1.61K
* **Visualizations:** Monthly Revenue Trends (Line Chart), Regional Performance (Column Chart), Product Category Breakdown, Sales Channel Share (Doughnut Chart), and Top 5 Products Ranking.
* **Interactivity:** Fully connected slicers for Region, Product Category, Sales Channel, Customer Type, and temporal drill-downs (Years, Quarters, Months, Days).

## 🛠️ Data Cleaning & ETL Process
The project began with a raw, intentionally messy sales dataset containing multiple real-world data quality issues:
* **Data Quality & Anomalies:** Resolved missing values, pricing anomalies, and data type mismatches across the table.
* **Text Normalization:** Standardized category, customer, and region text strings by eliminating trailing spaces and fixing casing inconsistencies using `=PROPER(TRIM(...))` formulas.
* **Date Handling & Helper Columns:** Addressed date format issues and engineered temporal helper columns (Years, Quarters, Months, Days) to bypass Excel Online's lack of automatic date-grouping in Pivot menus.
* **Cache Management:** Cleaned up PivotTable cache ghost items caused by pre-cleaned duplicate entries to ensure accurate slicer behavior.

## 💡 References & Inspiration
* Built following data visualization, formatting, and dashboard layout principles inspired by **Marg Analytics**.