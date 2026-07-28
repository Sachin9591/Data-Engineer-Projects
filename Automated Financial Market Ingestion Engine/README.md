# Automated Financial Market Ingestion Engine

An automated ETL pipeline designed to ingest, normalize, and validate live financial market data for analytical consumption.

## 📌 Features
- **Automated Market Ingestion:** Fetches real-time ticker data, trade volumes, and price fluctuations across multiple financial asset classes.
- **Data Validation & Cleaning:** Enforces strict schema validations and missing-value imputation before persistent storage.
- **High-Performance Transformation:** Uses **Polars** vectorization for sub-second data processing and indicator calculations.
- **Analytical Storage:** Persists cleaned market snapshots into DuckDB for fast historical backtesting and downstream reporting.

## 🛠️ Tech Stack
- **Language:** Python 3.14+
- **Data Processing:** Polars, NumPy
- **Database Engine:** DuckDB
- **Automation:** Python Schedule / Cron

## 🚀 Quick Start
1. Install dependencies:
   ```bash
   pip install "polars[rtcompat]" duckdb requests
