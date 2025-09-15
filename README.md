# ADF_to_ADB_Incremental
End-to-end Azure pipeline using Data Factory for incremental ingestion and Databricks for Delta Lake-based ETL. Adopts Medallion architecture (Bronze/Silver/Gold), building a Star Schema gold layer. Features modularity, parameterization, schema evolution, and performance best practices.

Azure End-to-End Data Engineering Project

This project demonstrates a complete Azure Data Engineering pipeline implementing the Medallion Architecture (Bronze → Silver → Gold) with incremental data loading and a Star Schema as the Gold layer.

🚀 Key Features

Incremental data load using Azure Data Factory (ADF) with watermarking.

Data transformation and curation in Azure Databricks (ADB) using PySpark and Delta Lake.

Star Schema (Gold Layer) with fact and dimension tables for analytics.

Infrastructure as Code with Bicep templates.

Centralized governance using Unity Catalog.

🏗️ Architecture

Source Data → GitHub CSV / Azure SQL Database

ADF Pipelines → Ingest initial & incremental data into Data Lake (Bronze)

Databricks ETL → Transform Bronze → Silver → Gold

Gold Layer → Star Schema optimized for BI tools like Power BI
⚡ Workflow

Initial Load – ADF copies data from GitHub/SQL DB to Data Lake (Bronze).

Incremental Load – ADF uses watermark table to bring only new data.

Silver Layer – Databricks cleans and transforms raw data into Delta tables.

Gold Layer – Star Schema built with fact & dimension tables.

📊 Star Schema

Fact Table – fact_sales

Dimensions – dim_model, dim_branch, dim_dealer, dim_date
<img width="1315" height="400" alt="image" src="https://github.com/user-attachments/assets/cd7e0eef-c5d3-4303-ad05-35d7e13efc7a" />

<img width="1486" height="751" alt="image" src="https://github.com/user-attachments/assets/babf5353-e5ae-43c8-a7f4-85cec0bca538" />
<img width="1169" height="686" alt="image" src="https://github.com/user-attachments/assets/b2e4cb9a-fb36-4896-8635-cfb64f2754b8" />

