# Ride Sharing Data Engineering Pipeline

## Project Overview

This project demonstrates an end-to-end Data Engineering Pipeline using **PySpark** and the **Medallion Architecture (Bronze, Silver, Gold)**.

The pipeline processes ride-sharing data from raw CSV files, transforms and cleans the data, and generates business-ready analytics.

---

## Technologies Used

- Python
- PySpark
- Google Colab
- Google Drive
- Git
- GitHub

---

## Project Structure

```
Ride_Sharing/
│
├── data/
│   ├── raw/
│   │   ├── drivers.csv
│   │   ├── trips.csv
│   │   └── trip_logs.csv
│   │
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── notebooks/
│   ├── 01_bronze.ipynb
│   ├── 02_silver.ipynb
│   └── 03_gold.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Bronze Layer

- Read raw CSV files
- Validate schema
- Store data in Parquet format

---

## Silver Layer

- Remove duplicate records
- Handle null values
- Join datasets
- Calculate trip duration
- Generate completion status
- Classify driver performance

---

## Gold Layer

Business analytics generated:

- Total Revenue
- Revenue by Driver
- Top 10 Drivers
- Revenue by City
- Most Popular Pickup Locations
- Cancellation Analysis
- Average Trip Duration
- Driver Ranking using Window Functions
- Delay Analysis

---

## Dataset

The project uses three datasets:

- Drivers
- Trips
- Trip Logs

---

## How to Run

1. Clone the repository.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebooks in Google Colab or Jupyter Notebook.
4. Run the notebooks in the following order:

```
01_bronze.ipynb
02_silver.ipynb
03_gold.ipynb
```

---

## Architecture

```
Raw CSV Data
      │
      ▼
 Bronze Layer
      │
      ▼
 Silver Layer
      │
      ▼
 Gold Layer
```

---

## Author

**Khushi Singh**