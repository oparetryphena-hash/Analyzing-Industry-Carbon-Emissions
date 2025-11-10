# Analyzing-Industry-Carbon-Emissions
 PostgreSQL project analyzing industry-level carbon emissions using The Carbon Catalogue dataset.
*Photo by Maxim Tolchinskiy on Unsplash*

## 📘 Overview

This project analyzes product-level carbon emissions (Product Carbon Footprints – PCFs) across industries using PostgreSQL. The goal is to understand which industries, companies, and countries contribute most to global emissions — and how emissions differ by product and production stage.

The dataset comes from **The Carbon Catalogue** (Nature.com), which provides verified greenhouse gas emissions data for various consumer and industrial products.

## 🧾 Dataset Information

**Table:** `product_emissions`

| Field | Description | Type |
|-------|--------------|------|
| `id` | Unique identifier | VARCHAR |
| `year` | Year of data | INT |
| `product_name` | Product name | VARCHAR |
| `company` | Company name | VARCHAR |
| `country` | Country of origin | VARCHAR |
| `industry_group` | Industry classification | VARCHAR |
| `weight_kg` | Product weight (kg) | NUMERIC |
| `carbon_footprint_pcf` | Total carbon footprint (kg CO₂e) | NUMERIC |
| `stage_emission` | Emission stage (e.g., production, use, end-of-life) | VARCHAR |

##  Tools Used

- **PostgreSQL** – for database creation, queries, and analysis  
- **Jupyter Notebook** – for documentation and visualization of SQL queries

## SQL Techniques Applied

- Data filtering and grouping using `GROUP BY` and `HAVING`  
- Window functions to compare emissions between products and companies  
- Common Table Expressions (CTEs) for structured analysis  
- Joins for comparing emissions across countries and industry groups  
- Aggregate functions (`SUM`, `AVG`, `MAX`) for summary insights  

  ## Key Insights

* Manufacturing and material extraction stages contribute the highest share of total emissions across industries.
* Certain industries like transportation and food processing have significantly higher average carbon footprints per kilogram.
* Products from developed countries tend to have lower emissions per product unit, possibly due to advanced technology and efficiency.
* The top 5 companies by carbon footprint accounted for nearly 40% of total emissions in the dataset.

##  Conclusion

This project highlights how SQL can be used for environmental and sustainability analytics, turning raw emission data into actionable insights for policymakers and companies aiming to reduce their carbon impact.

  

