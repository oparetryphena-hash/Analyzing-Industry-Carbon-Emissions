# Analyzing-Industry-Carbon-Emissions
 PostgreSQL project analyzing industry-level carbon emissions using The Carbon Catalogue dataset.
![Factories creating emissions](pollution.jpg)
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
  

