# NYC Yellow Taxi Data Cleaning Pipeline

This repository contains a Python-based data cleaning and preprocessing pipeline for the NYC Yellow Taxi Trip Records dataset.  
The cleaned dataset is designed for downstream analytics and visualization using Tableau Public.

---

## 📊 Dataset

- **Source:** NYC Taxi & Limousine Commission (TLC)
- **Data Type:** Yellow Taxi Trip Records (monthly Parquet files)
- **Format:** Parquet (raw) → CSV (cleaned)

Due to Tableau Public limitations with Parquet files, the raw data is converted and cleaned using Python before visualization.

---

## 🛠️ Tech Stack

- Python
- pandas
- pyarrow
- Jupyter Notebook (EDA)
- Tableau Public (downstream visualization)

---

## 🧹 Data Cleaning & Feature Engineering

The pipeline performs the following steps:

- Merges multiple monthly Parquet files
- Filters invalid trips (distance, fare, duration)
- Converts datetime fields
- Creates analytical features:
  - Pickup hour
  - Pickup weekday
  - Trip duration (minutes)
- Maps payment type codes to readable labels
- Joins taxi zone lookup data for location context
- Exports a Tableau-ready CSV file

---

