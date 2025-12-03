# Global-Superstore-Sales-Analysis
End-to-end Business Intelligence solution analyzing retail profitability using Power BI.

## Project Overview
**Role:** Business Intelligence Analyst  
**Tools:** Power BI, Power Query, DAX  
**Dataset:** Global Superstore Data (50,000+ records)

## Business Problem
A global retail giant is experiencing high sales volume but stagnant profitability. The management team needed a dynamic dashboard to identify loss-making products and regions to optimize their pricing strategy.

## The Solution
I built an interactive Power BI dashboard that enables stakeholders to:
1. Track **Year-over-Year (YoY)** growth for Sales and Profit.
2. Identify the **"Profit Traps"** (products with high sales but negative margins).
3. Analyze regional performance using a dynamic heatmap.

## Technical Steps
* **Data Transformation (ETL):** Used Power Query to clean data, handle nulls, and create a conditional "Delivery Status" column.
* **Data Modeling:** Designed a **Star Schema** with a dedicated Date Table for accurate time-intelligence analysis.
* **DAX Measures:** Created complex measures including:
    * `Sales YoY%` (Time Intelligence)
    * `Dynamic Ranking` (RANKX for Top 5 Products)
    * `Profit Margin` with conditional logic.
* **UX/UI:** Designed a navigation-friendly report with bookmarks, page navigation, and dynamic titles.

## Key Insights
* **The "Tables" Category Issue:** Despite being a top 5 revenue generator, "Tables" are operating at a **negative profit margin** in the West Region.
* **Shipping Impact:** "Same Day" shipping has the lowest profit margin, suggesting a need to restructure shipping costs.

## Dashboard Visuals
![Dashboard Screenshot]([# Global Superstore Sales Analysis](https://github.com/nuwanihitibandara211-wq/Global-Superstore-Sales-Analysis/blob/main/screenshots/Screenshot%202025-12-03%20170127.png))

