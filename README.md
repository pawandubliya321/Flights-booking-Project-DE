# Flight Booking Data Engineering Pipeline

## 📌 Project Overview
This project demonstrates an end-to-end Data Engineering pipeline
built on Google Cloud Platform (GCP) to process and analyze
flight booking data using modern cloud tools.

The pipeline is fully automated using Apache Airflow
and processes data using Dataproc Serverless (Spark),
finally loading curated data into BigQuery for analytics.

---

## 🏗 Architecture

Source (CSV files in GCS)
        |
        v
Dataproc Serverless (Spark)
        |
        v
BigQuery (Analytics Layer)
        |
        v
Airflow (Orchestration)

---

## ⚙️ Tech Stack

- Google Cloud Storage (GCS)
- Apache Airflow (Cloud Composer)
- Dataproc Serverless (PySpark)
- BigQuery
- GitHub Actions (CI/CD)

---

## 🔄 Pipeline Flow

1. Airflow triggers Dataproc Serverless batch job
2. Spark job reads raw flight booking data from GCS
3. Data is cleaned and transformed using PySpark
4. Final curated data is written to BigQuery tables
5. Airflow monitors job status and retries on failure

---

## 🚀 CI/CD

GitHub Actions is used to:
- Deploy Airflow DAGs to Composer
- Upload Spark jobs to GCS
- Manage environment-specific variables (dev/prod)

---

## 📊 Use Case

This pipeline enables:
- Analysis of flight booking trends
- Popular routes and airlines
- Revenue and demand insights

---

## 👨‍💻 Author
Pawan Dubliya Gurjar  
Aspiring Data Engineer
