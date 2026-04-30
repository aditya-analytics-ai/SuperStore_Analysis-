# Superstore Sales Analysis 
End-to-End Data Analysis Project
A complete data analysis project on a Superstore's sales data — covering data cleaning, 3 business dashboards (Customer, Product, and Time Series), and deep profitability insights.

# Project Structure
├── Sample_Superstore.csv              # Raw sales data
├── Superstore_Cleaned.csv             # Cleaned data (output of Store_sales_cleaning.ipynb)
├── Store_sales_cleaning.ipynb         # Data cleaning notebook
└── SuperStroreSales_dashboard.ipynb   # 3 dashboards + analysis notebook

# Project Overview
This project analyzes a retail Superstore's transactional data to uncover business insights across three dimensions:

Customer — who is buying, how loyal they are, and which customers drive profit
Product — which categories and sub-categories are profitable vs. loss-making
Time — how sales trend monthly, quarterly, and yearly, and how fast orders ship


## Part 1 – Data Cleaning (Store_sales_cleaning.ipynb)
The raw Sample_Superstore.csv dataset was cleaned through the following steps:
StepWhat was doneColumn name fixReplaced spaces with underscores across all column namesDate parsingConverted Order_Date and Ship_Date to proper datetime formatPostal code fixZero-padded Postal_Code to ensure 5-digit formatProduct name trimStripped leading/trailing whitespace from Product_NameDuplicate removalDropped duplicate rows based on Order_ID + Product_IDLoss-row inspectionExamined negative-profit rows (high discount impact)Column dropsRemoved Country (single value) and Row_ID (irrelevant index)Feature engineeringCreated Days_to_Ship, Order_Year, Order_Month, Order_Quarter
Output: Superstore_Cleaned.csv — a clean, analysis-ready dataset.

## Part 2 – Dashboards (SuperStroreSales_dashboard.ipynb)
Three fully consolidated dashboards were built, each with KPI cards + multiple charts in a single figure.

## Dashboard 1 – Customer-Centric Analysis
KPI Cards: Total Customers · Total Orders · Avg Order Value · Repeat Customer Rate
ChartWhat it showsSales & Profit by SegmentConsumer vs Corporate vs Home OfficeSales & Profit by RegionEast, West, South, Central comparisonTop 10 Customers by ProfitHighest value customersBottom 10 Customers by ProfitLoss-making customersCustomer Loyalty – Order FrequencyHow many orders each customer placedTop 10 States by SalesBest performing US states

## Dashboard 2 – Product-Centric Analysis
KPI Cards: Total Products · Total Revenue · Overall Profit Margin · Top Category
ChartWhat it showsSales & Profit by CategoryFurniture vs Office Supplies vs TechnologyProfit Margin (%) by CategoryWhich category earns more per dollar soldTop 5 Sub-Categories by ProfitBest performing sub-categoriesBottom 5 Sub-Categories by ProfitLoss-making sub-categoriesDiscount vs Profit ScatterHow discounts damage profitabilityTop 10 Products by SalesHighest revenue products

## Dashboard 3 – Time Series Analysis
KPI Cards: Total Sales · Overall Growth % · Peak Month · Avg Ship Time
ChartWhat it showsMonthly Sales & Profit TrendFull timeline with 3-Month Rolling AverageYearly Sales & Profit ComparisonYear-by-year grouped bar chartYear-over-Year Sales Growth (%)Annual growth rate trendMonthly Seasonality PatternAvg sales per order by monthAvg Shipping Time by ModeFirst Class vs Second Class vs Standard

# Key Business Insights

✅ Consumer segment leads in total sales across all regions
✅ Technology is the most profitable category; Furniture has the lowest margin
✅ Tables and Bookcases are major loss-making sub-categories
✅ High discounts (>30%) consistently result in negative profit
✅ Q4 is the strongest quarter — clear seasonal spike in sales
✅ Standard Class shipping has the highest order volume but slowest delivery
✅ A significant portion of customers are repeat buyers, indicating good retention

# Author
Adityamohan Singh

GitHub: @your-username
LinkedIn: your-linkedin
