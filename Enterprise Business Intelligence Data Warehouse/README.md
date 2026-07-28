# Enterprise Business Intelligence Data Warehouse

An end-to-end OLAP data warehouse implementing Star Schema dimensional modeling to serve enterprise-level business intelligence reports.

## 📌 Features
- **Dimensional Modeling:** Built with Kimball methodology featuring centralized Fact tables and denormalized Dimension tables (`Dim_Customer`, `Dim_Product`, `Dim_Date`).
- **ETL Transformation Pipelines:** Extracts raw operational logs and transforms them into structured analytical datasets.
- **Columnar Storage Optimization:** Leverages **DuckDB** and **Parquet** columnar formats to achieve high compression and fast aggregate query execution.
- **BI Reporting Layer:** Provides pre-aggregated analytical views designed for seamless connection to dashboards (Tableau, PowerBI, Streamlit).

## 🛠️ Tech Stack
- **Data Warehousing:** DuckDB
- **Transformation Engine:** Polars, SQL
- **Storage Format:** Apache Parquet

## 🚀 Quick Start
1. Run the database initialization script:
   ```bash
   python Enterprise Business Intelligence Data Warehouse.py
