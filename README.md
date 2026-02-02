Databricks ETL & Data Warehouse Project
Overview

This project demonstrates an ETL pipeline using Databricks, Delta Lake, and Azure Data Lake Storage. Raw data is ingested, cleaned, and transformed into analytics-ready fact and dimension tables following a Bronze → Silver → Gold architecture.

Architecture

Bronze Layer: Raw, unprocessed data in Delta format.
Silver Layer: Cleaned and structured data, ready for transformation.
Gold Layer: Star-schema design for analytics with fact and dimension tables.

Fact Table: gold.fact_sales – contains sales metrics with product_key & customer_key.
Dimension Tables:

gold.dim_products – product details with surrogate keys

gold.dim_customers – customer demographics with surrogate keys

Storage: External Delta tables in ADLS for ACID transactions and schema evolution.

Tools & Technologies

Databricks, PySpark, SQL

Delta Lake, ADLS Gen2

Git & GitHub
