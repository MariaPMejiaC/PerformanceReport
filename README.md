# Plant Co. Sales Performance Report – Power BI Dashboard


## Overview
This Power BI dashboard was developed to replace traditional reporting methods with an interactive visual interface for the sales department at Plant Co. The dashboard enables detailed tracking and analysis of sales performance across countries, products, and customer accounts. It is designed to help business users and stakeholders monitor key sales indicators, evaluate profitability by segment, and identify underperforming markets to drive more informed strategic decisions.

# Business Objectives
- Transition from static Excel reports to dynamic, interactive dashboards.
- Provide a clear view of year-to-date (YTD) vs prior year-to-date (PYTD) performance.
- Enable deep-dive analysis by country, product, and account.
- Highlight profitability and sales contribution by product type and customer segments.
- Identify top/bottom-performing markets and trends over time.
- Support actionable decision-making on product focus and account strategy.

## Dashboard Features
✅ KPI Cards
- YTD Sales
- PYTD Sales
- Sales Difference (YTD vs PYTD)
- Gross Profit
- Gross Profit %

✅ Interactive Filters (Slicers)
- Year
- Product Type
- Date
- Country
- Value Type (Sales, Quantity, Gross Profit)

✅ Visuals & Charts
- Waterfall Chart: Highlights monthly YTD vs PYTD changes with increase/decrease annotations.
- Treemap: Bottom 10 countries by YTD vs PYTD performance.
- Clustered Bar Chart: Monthly sales trends segmented by product type (Indoor, Outdoor, Landscape).
- Line Chart Overlay: Tracks PYTD vs YTD comparison to monitor seasonal performance shifts.
- Scatter Plot: Profitability segmentation by account, showing GP% vs YTD sales value.

✅Custom Measures & DAX Calculations
- YTD_Sales, PYTD_Sales, YTD_GrossProfit, GP%
- Switch logic for dynamic value type switching (Sales, Quantity, GP)
- Monthly difference calculations (ΔYTD vs PYTD)
Ranking logic for identifying bottom 10 performing countries

## Development Process
#### Data Preparation
- Loaded and transformed data from multiple sources using Power Query.
- Ensured consistency in date formats, country codes, and product hierarchies.

#### Data Modeling
- Implemented a star schema with:
- Fact Table: Fact_Sales
- Dimension Tables: Dim_Account, Dim_Product, Dim_Date
- Relationships built based on keys like Account_id, Product_id, and Date.

#### DAX Measures
- Created reusable and dynamic measures for KPIs, trend comparisons, and profitability.
- Implemented a switching logic using a disconnected slicer table (Slc_Values) to control metric types.

#### Visualizations
- Designed clean, functional visuals with interactivity.
- Used conditional formatting and data labels to enhance clarity.
- Bookmarks and slicers added for better user navigation.

#### Deployment
- Published to Power BI Service with scheduled refresh.
- Shared access with Sales and Strategy teams for real-time tracking.

# Dashboard Overview
![Image](https://github.com/user-attachments/assets/8ab97940-a98a-4ea3-ad42-55deeec09fd2)
