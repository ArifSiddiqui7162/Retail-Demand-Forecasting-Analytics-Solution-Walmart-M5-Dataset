# Retail-Demand-Forecasting-Analytics-Solution-Walmart-M5-Dataset

## 📌 Project Overview

This project delivers an **end-to-end retail analytics and forecasting solution** using Walmart’s M5 competition dataset.  
The dataset contains multi-year, multi-store, multi-product sales, pricing, and event data across thousands of SKUs, offering realistic complexity for advanced analytics.

**Business Problem:**  
Walmart needs to improve **inventory management, demand forecasting, and promotion effectiveness** to minimize stockouts, reduce overstock costs, and maximize revenue.

**Solution Approach:**  
- Designed a **SQL Server data warehouse** with a star schema for efficient querying and analysis.  
- Conducted **Python-based exploratory data analysis (EDA)** and statistical hypothesis testing to uncover trends, seasonality, and price sensitivity.  
- Developed **machine learning forecasting models** to predict product-level daily demand.  
- Built **interactive Power BI dashboards** for executives, inventory managers, and marketing teams to track KPIs, monitor forecasts, and evaluate promotion performance.

**Goals:**  
- Increase forecast accuracy to improve inventory planning.  
- Identify high-impact promotions and optimize pricing strategies.  
- Provide actionable, data-driven insights for strategic retail decision-making.

## 🎯 Business Objectives

The primary objectives of this project are:

1. **Inventory Optimization**  
   - Reduce stockouts by accurately forecasting demand at the SKU-store level.  
   - Minimize overstock to lower holding costs and improve cash flow.  

2. **Demand Forecasting**  
   - Develop predictive models to forecast daily sales for thousands of SKUs across multiple stores.  
   - Account for seasonality, trends, holidays, and promotions to improve forecast accuracy.  

3. **Promotion ROI Analysis**  
   - Measure the effectiveness of promotional campaigns in driving sales.  
   - Calculate ROI for different promotion types to guide marketing spend.  

4. **Data-Driven Decision Support**  
   - Provide actionable insights to executives, inventory managers, and marketing teams through interactive dashboards.  
   - Enable scenario planning for pricing and promotion strategies.

## 📊 Dataset Variable to Business Context Mapping

This project uses the Walmart M5 Forecasting Competition dataset.  
The table below maps each key variable to its technical meaning, business relevance, and example use case.

| Dataset | Column Name | Technical Meaning | Business Context | Example Use Case |
|---------|------------|-------------------|------------------|------------------|
| calendar | `event_name_1` | Name of the first event/holiday on that day | Special days that can impact demand | Plan promotions or stock increases before holidays |
| calendar | `event_type_1` | Type of event (National holiday, Sporting event, etc.) | Helps categorize sales spikes | Analyze impact of different event types |
| sell_prices | `sell_price` | Price of an item in a store for a given week | Determines demand sensitivity (price elasticity) | Check if lowering prices increases sales |
| sell_prices | `wm_yr_wk` | Walmart’s year-week code | Aligns prices with sales weeks | Merge weekly price data with sales data |
| sales_train_validation | `d_1`–`d_1913` | Sequential day numbers for sales | Each corresponds to a real date | Match with holidays, promotions, or seasons |
| sales_train_validation | `item_id` | Unique product code | Identifies specific products | Track sales performance by product |
| sales_train_validation | `store_id` | Store location code | Links sales to physical locations | Compare performance between stores |
| calendar | `snap_CA`, `snap_TX`, `snap_WI` | SNAP (Supplemental Nutrition Assistance Program) activity in each state | Indicates when customers have more purchasing power | Target promotions during SNAP days |

> **Note:** Dates for `d_1`, `d_2`, ... are mapped via the `calendar` table.

## 🛠 Tools & Tech Stack

This project uses a combination of database, analytics, visualization, and machine learning tools:

- **SQL Server** – Data warehousing, star/snowflake schema design, ETL, and advanced SQL queries
- **Python** – Data cleaning, transformation, feature engineering, and modeling
  - **Pandas** – Data manipulation and EDA
  - **NumPy** – Numerical operations
  - **Scikit-learn** – Machine learning (classification, regression, clustering)
  - **Prophet** – Time series forecasting
  - **Matplotlib & Seaborn** – Data visualization
- **Power BI** – Interactive dashboard creation and KPI tracking
- **Jupyter Notebook** – Code experimentation and documentation
- **Git & GitHub** – Version control and project documentation

## 📅 Project Roadmap

The project will be executed in the following phases:

1. **Planning & Data Understanding**  
   - Define objectives, KPIs, and map dataset variables to business context.  

2. **Data Modeling & Warehouse Design**  
   - Create star/snowflake schema in SQL Server.  
   - Design ETL workflows.  

3. **ETL & Data Cleaning**  
   - Load datasets into SQL Server.  
   - Handle missing values, outliers, and data transformations.  

4. **Exploratory Data Analysis (EDA)**  
   - Perform statistical analysis, visualizations, and hypothesis testing.  

5. **Business Analytics & KPIs**  
   - Calculate stockout rate, promotion lift, inventory turnover, and other metrics.  

6. **Power BI Dashboard Development**  
   - Build interactive dashboards with drill-downs, filters, and KPIs.  

7. **Machine Learning Modeling**  
   - Forecast demand using time series models.  
   - Apply regression, classification, and clustering as needed.  

8. **Insights & Recommendations**  
   - Summarize business findings and link to objectives.  

9. **Documentation & Delivery**  
   - Prepare final README, code comments, and dashboard exports.
