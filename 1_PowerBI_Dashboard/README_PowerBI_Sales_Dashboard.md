Power BI Sales & Inventory Dashboard

Status: Completed / In Progress
Tools: Power BI, DAX, Power Query, SQL (optional), Excel / CSV dataset

📌 Project Overview

This dashboard was designed to demonstrate my ability to load, clean, model, and visualize business data using Power BI. It focuses on providing insights into sales performance, inventory movement, and key operational metrics important for data-driven decision-making.

The project mimics the type of BI reporting commonly used by organizations to track KPIs and optimize operations.

🎯 Objectives

Build a clean and optimized Power BI data model (star schema).

Create meaningful visuals for sales trends, product performance, and inventory levels.

Apply DAX measures for calculations such as YTD, YoY, variance %, and performance KPIs.

Improve performance with DAX optimization techniques.

Publish & share dashboard via Power BI Service.

📊 Key Features

Sales Trend Analysis with daily/weekly/monthly visuals

Top performing products & categories

Inventory levels monitoring

Interactive filters for date, region, product, etc.

Dynamic KPIs:

Total Sales

Average Order Value

Stock Coverage

Month-over-Month Growth

🧮 Sample DAX Measures
Total Sales = SUM(Sales[SalesAmount])

YoY Sales Growth = 
VAR CurrentYear = CALCULATE([Total Sales], YEAR(Sales[Date]) = YEAR(TODAY()))
VAR LastYear = CALCULATE([Total Sales], YEAR(Sales[Date]) = YEAR(TODAY()) - 1)
RETURN DIVIDE(CurrentYear - LastYear, LastYear)

📂 Data Model

Fact table: SalesFact

Dimension tables: Products, Calendar, Regions, Inventory

Includes relationships to support star schema modeling.

⚙️ Performance Optimization

Used variables inside DAX for faster calculations

Avoided row context where possible

Reduced cardinality

Disabled auto date/time

Compressed data types

📁 Files Included

PowerBI_Sales_Dashboard.pbix

Dataset(s)

Screenshots


📥 How to Use

Download the .pbix file

Open in Power BI Desktop

Refresh dataset and explore the visuals

💡 Future Improvements

Connect to a live SQL database

Add automated refreshes with Power Automate

Add forecasting using DAX + analytics tools

Add Power BI README
