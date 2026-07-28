# Real-Time E-Commerce Anomaly Engine

A high-throughput, single-threaded streaming pipeline built to detect fraud and high-value transactional anomalies in real time without external infrastructure dependencies.

## 📌 Features
- **In-Memory Streaming Producer:** Simulates real-time e-commerce events (views, cart adds, purchases) with synthetic anomaly injection using `Faker`.
- **Sliding Window Analytics:** Maintains an active 20-event rolling buffer to compute streaming metrics and trigger fraud alerts.
- **Embedded OLAP Storage:** Utilizes in-memory **DuckDB** for fast micro-aggregations and SQL-based anomaly identification.
- **Lakehouse Persistence:** Exports streaming batches directly into a partitioned **Parquet Lakehouse** (`event_type=...`) on disk.

## 🛠️ Tech Stack
- **Language:** Python 3.14+
- **Analytics & Storage:** DuckDB, Polars (`rtcompat`)
- **Data Generation:** Faker
- **Environment:** Interactive Jupyter Notebooks

## 🚀 Quick Start
1. Install dependencies:
   ```bash
   pip install "polars[rtcompat]" duckdb faker
