# Global Superstore Sales & Profitability Dashboard

## 📌 Project Overview
**Role:** Business Intelligence Analyst  
**Domain:** Retail / E-commerce  
**Tools:** Power BI, Power Query, DAX, Excel  
**Dataset:** [Sample - Superstore]([superstore dataset](https://github.com/nuwanihitibandara211-wq/Global-Superstore-Sales-Analysis/blob/main/Sample%20-%20Superstore.csv)) (9,994 records)

---

## 💼 Business Problem
A global retail giant has been experiencing high sales volume but inconsistent profitability across different regions. The management team needed a data-driven solution to answer three critical questions:
1. **Where are we losing money?** (Which regions/products are unprofitable?)
2. **How is our logistics performance?** (Are late shipments affecting business?)
3. **Which products drive the most growth?** (YoY analysis).

---

## 🛠️ The Solution
I designed an end-to-end Business Intelligence solution that transforms raw sales data into actionable insights.

### 1. Data Transformation (ETL)
* **Data Cleaning:** Used Power Query to check for nulls and correct data types.
* **Custom Logic:** Created a conditional column `Delivery Status` to flag orders where `Ship Date - Order Date > 5 days`.
* **Date Table:** Generated a dynamic `DateTable` using DAX to support time-intelligence functions.

### 2. Data Modeling
* Built a **Star Schema** data model to optimize performance.
* Established **One-to-Many** relationships between the Fact Table (Sales) and Dimension Tables (Date, Location).

### 3. Advanced DAX Measures
I moved beyond simple aggregations to create complex business logic:
* **Profit Margin %:** `DIVIDE([Total Profit], [Total Sales], 0)`
* **Dynamic Ranking:** `RANKX` to identify the Top 5 performing products dynamically based on slicer selection.
* **YoY Growth:** Used `CALCULATE` and `SAMEPERIODLASTYEAR` to compare performance against the previous year.
* **Conditional Formatting:** Applied logic to flag negative profit margins in Red and positive in Green.

---

## 📉 Key Insights Revealed
1.  ** The "Tables" Trap:** While "Tables" are a top revenue generator in the **West Region**, they are operating at a massive loss (Negative Profit Margin), suggesting a need for immediate repricing or discontinuation.
2.  **Shipping Bottlenecks:** Analysis of the new `Delivery Status` metric showed that **Standard Class** shipments have the highest delay rate, correlating with lower customer retention in specific cities.
3.  **Seasonality:** Sales consistently spike in **November/December**, but profit margins dip due to heavy discounting.

---

## 📸 Visuals & Dashboard
*(Please upload your screenshots to a folder named 'screenshots' and link them below)*

### Main Dashboard
![Main Dashboard](screenshots/dashboard_image1.png)

---

## 🚀 How to Run This Project
1.  Download the `.pbix` file from this repository.
2.  Open in **Power BI Desktop**.
3.  Interact with the Year/Region slicers to filter the data.

---

## 👤 Author
**[Your Name]** [Link to your LinkedIn Profile]
