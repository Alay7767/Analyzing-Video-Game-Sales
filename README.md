# 🎮 Video Game Sales Analysis

This project analyzes video game sales data to uncover trends across regions, platforms, and genres.  

Using **Power BI** for data cleaning and **Tableau** for visualization, the project transforms unstructured data into actionable insights for game publishers and retailers/distributors.

---

## 📌 Project Overview

**Goal:**  
Transform unstructured Excel data into a clean, structured dataset and build interactive dashboards to support data-driven decision-making.

**Data Source:**  
`vgsales.csv` (initially uncleaned and unstructured)

### 🛠️ Tools Used

| Tool      | Purpose |
|-----------|----------|
| Power BI  | Data cleaning & transformation |
| Excel     | Storage of cleaned dataset |
| Tableau   | Interactive dashboards & visualization |

---

## 🧹 Data Preprocessing (Power BI - Power Query Editor)

The following steps were performed:

- Imported raw data from `vgsales.csv`
- Converted sales columns (`NA_Sales`, `EU_Sales`, `JP_Sales`, `Other_Sales`, `Global_Sales`) into actual unit sales
- Removed duplicates based on:
  - Name
  - Platform
  - Year
  - Genre
  - Publisher
- Handled missing values by replacing them with `"Unknown"` or mode values
- Trimmed and cleaned text fields (`Name`, `Genre`, `Publisher`)
- Converted data types:
  - `Year` → Whole Number  
  - Sales Columns → Decimal Number
- Created new column:
Total_Sales = NA_Sales + EU_Sales + JP_Sales + Other_Sales
