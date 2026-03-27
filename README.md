# AdventureWorks Cycles – Power BI Sales & Customer Dashboard

## Business Problem

The sales and marketing teams at AdventureWorks Cycles lacked a centralized, interactive view of their global operations. They faced challenges such as:

- **Understanding customer behavior** – Who are the top customers? What are the demographics (age, income, occupation) of our most profitable segments?
- **Monitoring product performance** – Which products generate the highest revenue? Which have concerning return rates that may indicate quality issues?
- **Tracking financial health** – How do revenue, profit, and cost trend over time? Can we drill down from year to day to spot anomalies?
- **Identifying regional opportunities** – Where are our sales strongest, and which territories need more attention?

The goal was to build a self-service BI solution that empowers stakeholders to explore these questions without relying on static Excel reports or IT intervention.

## Solution Overview

I developed an interactive Power BI dashboard that transforms raw sales, customer, product, and returns data into actionable insights. The report includes:

- An **Executive Summary** with high-level KPIs, category performance, and financial trends.
- A **Customer Details** page for segmentation and top‑customer analysis.
- A **Product Details** page for deep dives into individual product revenue and returns.
- A **Global Sales Map** to visualize performance by country and continent.

All pages are fully interactive, allowing users to filter by time, geography, and product category.

## Skills Demonstrated

- **Data Modeling** – Designed a star schema with fact tables (`Sales Data`, `Returns Data`) and dimension tables (`Calendar`, `Customer`, `Product`, `Territories`) to support efficient, cross‑filtered analysis.
- **DAX (Data Analysis Expressions)** – Created measures for key metrics: Total Revenue, Return Rate, Month‑over‑Month growth, and dynamic time‑intelligence calculations.
- **Data Visualization** – Built intuitive, visually consistent reports with attention to layout, color coding, and user experience.
- **Interactive Design** – Implemented slicers, drill‑through pages, and cross‑filtering to enable ad‑hoc exploration.
- **Business Storytelling** – Structured the dashboard to guide users from high‑level summaries down to granular details, answering specific business questions.

## Tools Used

- **Microsoft Power BI Desktop** – Report development, data modeling, and DAX.
- **Power Query** – Data transformation and cleaning (assumed from source data preparation).
- **DAX Studio** (optional) – For advanced measure debugging and optimization.

## Data Model Summary

The model follows a star schema:

- **Fact Tables**  
  - `Sales Data`: transactional orders (OrderNumber, Quantity, Revenue, CustomerKey, ProductKey, OrderDate)  
  - `Returns Data`: returned quantities linked to ProductKey, ReturnDate, TerritoryKey

- **Dimension Tables**  
  - `Calendar`: date hierarchy for time intelligence  
  - `Customer`: demographics, income, customer priority  
  - `Product_lookup` & related category/subcategory tables: product details and hierarchy  
  - `Territories Lookup`: continent, country, region

Relationships ensure that filters on any dimension propagate correctly across all visualizations.

## Key Features & Insights

- **Executive Summary**  
  - Total Revenue: **$18.51M**  
  - Monthly Revenue trend with previous month comparison  
  - Orders by Category & Gender  
  - Top 10 products by orders with return rates  
  - Revenue, Profit, and Cost drill‑down (Year → Quarter → Month → Day)

- **Customer Insights**  
  - Top customers by revenue and total orders  
  - Demographic breakdowns (gender, income level, occupation)  
  - Revenue vs. orders over time  
  - Order distribution by age group

- **Product Insights**  
  - Select any product to view its monthly/weekly revenue and return trends  
  - Identify seasonal patterns and potential quality issues

- **Geographic Analysis**  
  - Global sales distribution
  - Region-based filtering (North America, Europe, Pacific)
  - Market-level insightsInteractive map showing sales by country and continent, highlighting market penetration
    
- **Key Insights**
  - North America generates the highest revenue contribution
  - Certain products show elevated return rates
  - Revenue demonstrates steady growth with periodic spikes
  - A small segment of customers drives a large portion of revenue
  - Product demand varies significantly by region

## How to Use This Repository

1. **Download** the `.pbix` file (if included in the repository).
2. **Open** with Power BI Desktop (free version available from Microsoft).
3. **Explore** – Use slicers (date, continent, product category) to filter all pages. Click on any visual to cross‑highlight related data.
4. **Drill‑through** – Right‑click on a data point (e.g., a customer name) to navigate to a detailed view.

## Conclusion

This Power BI project demonstrates a complete business intelligence workflow: from understanding business requirements, building a robust data model, writing advanced DAX, to delivering a user‑friendly, interactive dashboard. It empowers decision‑makers at AdventureWorks Cycles to quickly answer critical questions about sales performance, customer behavior, and product quality.

📬 Contact

If you need a similar Power BI dashboard or BI solution:

Fiverr: https://www.fiverr.com/s/BRVNWW1,https://www.fiverr.com/s/2KR860X
LinkedIn: https://www.linkedin.com/in/bazghawaqas/
---

*Thank you for reviewing my work. For more projects, please visit my GitHub profile.*
