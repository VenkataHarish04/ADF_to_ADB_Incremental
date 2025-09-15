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
