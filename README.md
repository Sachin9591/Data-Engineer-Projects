# 🛠️ Data Engineering Portfolio

Welcome to my Data Engineering project repository. This collection demonstrates production-grade ETL pipelines, real-time stream processing, and analytical data warehousing using modern, lightweight Python architectures (**DuckDB**, **Polars**, and **Apache Parquet**).

---

## 📌 Projects Overview

| Project | Primary Focus | Key Technologies | Storage / Format |
| :--- | :--- | :--- | :--- |
| **[Real-Time E-Commerce Anomaly Engine](./Real-Time%20E-Commerce%20Anamoly%20Engine)** | Stream Processing & Fraud Detection | Python 3.14+, DuckDB, Polars, Faker | In-Memory & Partitioned Parquet |
| **[Automated Financial Market Ingestion Engine](./Automated%20Financial%20Market%20Ingestion%20Engine)** | High-Frequency Market ETL | Python, Polars (`rtcompat`), DuckDB, APIs | DuckDB OLAP Storage |
| **[Enterprise Business Intelligence Data Warehouse](./Enterprise%20Business%20Intelligence%20Data%20Warehouse)** | Star Schema & Dimensional Modeling | DuckDB, Polars SQL, Kimball Methodology | Columnar Parquet Files |

---

## 🚀 Key Architectural Highlights

* **In-Process OLAP Computing:** Built using **DuckDB** and **Polars** to achieve sub-second analytical query performance without high-overhead Docker containerization or JVM cold starts.
* **Stream-to-Lakehouse Pipeline:** Implements low-latency sliding-window aggregation with automated partitioned Parquet exports.
* **Robust Hardware Compatibility:** Configured specifically to run safely on high-performance vector-processing environments using runtime-compatible Polars builds.

---

## 📂 Repository Structure

```text
Data Engineer Projects/
│
├── Real-Time E-Commerce Anamoly Engine/
│   ├── Real-Time E-Commerce Anamoly Engine.ipynb
│   ├── data/parquet_lakehouse/
│   └── README.md
│
├── Automated Financial Market Ingestion Engine/
│   ├── Automated Financial Market Ingestion Engine.py
│   ├── data/
│   └── README.md
│
├── Enterprise Business Intelligence Data Warehouse/
│   ├── Enterprise Business Intelligence Data Warehouse.py
│   ├── queries/
│   └── README.md
│
└── README.md (Root)
