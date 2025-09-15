# ADF_to_ADB_Incremental
End-to-end Azure pipeline using Data Factory for incremental ingestion and Databricks for Delta Lake-based ETL. Adopts Medallion architecture (Bronze/Silver/Gold), building a Star Schema gold layer. Features modularity, parameterization, schema evolution, and performance best practices.
Azure-End-To-End-Data-Engineering-Project/
├── data/                   # Sample datasets (initial & incremental)
├── docs/                   # Diagrams + setup guides
├── azure-setup/            # Bicep templates for infra provisioning
├── sql-scripts/            # SQL for watermark & source tables
├── adf-pipelines/          # Linked services, datasets, pipelines
├── databricks-notebooks/   # PySpark ETL notebooks for Silver & Gold
├── databricks-workflows/   # Workflow JSON for orchestration
├── README.md               # Project documentation
└── LICENSE                 # License file
