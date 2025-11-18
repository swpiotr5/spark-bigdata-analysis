📊 Citibike Big Data Analytics — Apache Spark Project
🚴‍♂️ Analysis of New York Citibike Trips Using Apache Spark
⚡ High-performance ETL • Big Data Storage • Distributed Processing
📌 Project Overview

This project implements a full Big Data processing pipeline using Apache Spark, focusing on large-scale analysis of the Citibike NYC trip dataset.
The goal is to showcase the installation, configuration, storage, transformation, and exploration of massive datasets using modern distributed tools.

The dataset contains huge amount of records per year and is used to demonstrate:

- High-volume data ingestion

- Distributed processing with Spark

- Cleaning & harmonization of inconsistent schemas

- Storage in optimized formats (Parquet)

- Building a scalable analytical environment

🚀 Key Features

✔️ Full Big Data environment using Apache Spark
✔️ ETL pipeline for ingesting, cleaning and merging rows
✔️ Handling schema inconsistencies (e.g., duplicate 2017 columns)
✔️ Storage in multiple formats: CSV, Parquet
✔️ Efficient querying using Spark SQL
✔️ Support for local Docker-based analytics environment
✔️ Exploratory analysis & visualizations

🧱 Tech Stack
| Category              | Tools                                    |
| --------------------- | ---------------------------------------- |
| **Processing Engine** | Apache Spark (PySpark)                   |
| **Environment**       | JupyterLab • Docker • Python 3.10        |
| **Storage Formats**   | CSV, Parquet                             |
| **Libraries**         | pandas, matplotlib, seaborn, pyspark.sql |
| **Data Source**       | Citibike NYC Trip Data                   |

🐳 Project Architecture
```text
+---------------------------+
|        User (You)         |
|      Jupyter Notebook     |
+-------------+-------------+
              |
              v
+---------------------------+
|       Apache Spark        |
|  Distributed Processing   |
+-------------+-------------+
              |
              v
+---------------------------+
|   Data Lake / File Store  |
|    CSV  |  Parquet        |
+---------------------------+
```

📂 Directory Structure

```text
citibike-bigdata/
│
├── docker/
│   └── docker-compose.yml        # Spark + Jupyter environment
│
├── notebooks/
│   └── citibike_analysis.ipynb   # Main analysis notebook
│
├── data/
│   ├── citibike/                 # Raw yearly/monthly data
│   └── citibike_merged/          # Cleaned & merged yearly files
│
└── README.md
```

🔥 What This Project Demonstrates
🟦 1. Setting up Apache Spark locally (Docker)

Spark master + worker

JupyterLab with PySpark

Shared volume for easy development

🟩 2. ETL: Loading millions of rows

Recursive scanning of year/month folders

Detecting & fixing inconsistent schemas

Handling malformed CSVs

Merging datasets into a unified yearly DataFrame

🟨 3. Saving to high-performance formats

Efficient Parquet dumps

Automatic schema enforcement

Compression + optimized storage

🟧 4. Data exploration

🏁 How to Run the Project

1️⃣ Clone repo

git clone https://github.com/swpiotr5/spark-bigdata-analysis.git
cd citibike-bigdata

2️⃣ Start Spark + Jupyter

docker compose up

3️⃣ Open Jupyter

http://localhost:8888

4️⃣ Run notebook

notebooks/citibike_analysis.ipynb


