# Analyzing-Video-Game-Sales

🎮 Video Game Sales Analysis

This project analyzes video game sales data to uncover trends across regions, platforms, and genres. Using Power BI for data cleaning and Tableau for visualization, the project transforms unstructured data into actionable insights for game publishers and retailers/distributors.

📌 Project Overview

Goal: Turn unstructured Excel data into a clean, structured dataset and build interactive dashboards to support data-driven decisions.

Data Source: vgsales.csv (initially uncleaned and unstructured).

Tools Used:

Power BI: Data cleaning, transformation, and preprocessing.

Excel: Storage of cleaned data.

Tableau: Interactive dashboards and visualizations.

🧹 Data Preprocessing

We performed data cleaning and transformation in Power BI using Power Query Editor:

Imported raw data from vgsales.csv.

Converted sales columns (NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales) to actual unit sales.

Removed duplicates based on Name, Platform, Year, Genre, and Publisher.

Handled missing values by replacing them with 'Unknown' or mode values.

Trimmed and cleaned text fields (Name, Genre, Publisher).

Converted data types:

Year → Whole Number

Sales Columns → Decimal Number

Created a new column Total_Sales = NA_Sales + EU_Sales + JP_Sales + Other_Sales.

Filtered out rows with incomplete or invalid critical data.

The cleaned dataset was then exported back to Excel for visualization in Tableau.

❓ Business Questions Answered
📝 For Game Publishers

Which game has the highest global sales in the dataset?

How do sales differ by region (North America, Europe, Japan, etc.)?

Which platforms are most popular for game releases?

How does the sales performance of games compare to competitors in the same genre?

What is the sales trend over time for top games, and how do these compare across regions?

Which genres have the highest sales, and which regions show the most interest in each genre?

🛒 For Retailers & Distributors

Which platforms have the highest sales worldwide, and how do these vary by region?

Which genres are the top sellers in North America versus Europe and Japan?

How do the sales of top-selling games compare across regions?

What have been the sales trends for games over the last five years in different regions?

Which platform has shown the most growth in sales over the last decade?

What are the most popular game genres across all regions, and which are emerging as popular trends?

📊 Dashboard Visualizations
Plot Type	Question Addressed	Description
Bar Chart	Top 10 best-selling games by Global Sales	Ranks the top 10 games by total global sales.
Stacked Column	Regional sales comparison for top platforms	Compares sales of leading platforms segmented by region (NA, EU, JP, Other).
Pie Chart	Market share by game genre	Shows the proportion of total sales by each genre.
Line Chart	Sales trend over years per region	Plots annual sales for each region to reveal trends over time.
TreeMap	Sales distribution by Platform and Genre	Displays sales volume grouped by platform and genre.
Heatmap	Platform popularity by region	Highlights which platforms are most popular in each region.
Clustered Bar	Genre-wise sales by region	Compares sales for each genre across regions.
Area Chart	Emerging genre trends over time	Displays cumulative sales by genre, showing rising or declining genres.
Scatter Plot	Top-selling genres in NA, EU, and Japan	Shows regional preferences and popular genre trends.
🖱️ Dashboard Interactivity

The Tableau dashboard includes interactive filters and controls:

Genre Filter – Filter visualizations by selected genres.

Year Range Slider – Dynamic filtering of data by release year.

Region Selector – Toggle between NA, EU, JP, and Global data.

Platform Filter – Compare specific platforms across multiple charts.

These controls allow users to explore insights interactively.

🛠️ Tools Used
Tool	Purpose
Power BI	Data cleaning & transformation
Excel	Cleaned dataset storage
Tableau	Interactive dashboards & visualization
📂 Project Structure
📁 data/
   ├── raw/vgsales.csv
   ├── cleaned/vgsales_cleaned.xlsx
📁 powerbi/
   └── cleaning_steps.pbix
📁 tableau/
   └── vgsales_dashboard.twbx
📁 images/
   └── dashboard_mockups.png
README.md

🚀 Results

Clean, structured dataset for video game sales.

Interactive Tableau dashboards answering key business questions.

Actionable insights into sales trends, platform performance, and genre popularity.

📌 Future Improvements

Automate data cleaning with Python or R.

Integrate real-time sales data for live dashboards.

Add additional datasets (e.g., reviews, ratings) for richer analysis.
