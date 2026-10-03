# 🎬 Netflix End-to-End Data Engineering Pipeline

![Azure](https://img.shields.io/badge/Azure-Cloud-blue)
![ADF](https://img.shields.io/badge/Azure%20Data%20Factory-Data%20Integration-blue)
![Databricks](https://img.shields.io/badge/Azure%20Databricks-Data%20Engineering-red)
![PySpark](https://img.shields.io/badge/PySpark-Processing-orange)
![Delta Lake](https://img.shields.io/badge/Delta%20Lake-Storage-purple)
![ADLS Gen2](https://img.shields.io/badge/ADLS%20Gen2-Data%20Lake-blue)
![Python](https://img.shields.io/badge/Python-3.x-yellow)
![SQL](https://img.shields.io/badge/SQL-Analytics-lightgrey)
![GitHub](https://img.shields.io/badge/GitHub-Version%20Control-black)

---

## 📌 Project Overview

This project implements an **end-to-end cloud data engineering pipeline** for processing Netflix Movies and TV Shows data using Microsoft Azure services.

The solution demonstrates how raw datasets can be ingested, stored, cleaned, transformed, modeled, and converted into analytics-ready datasets using a modern cloud data engineering architecture.

The pipeline is orchestrated using **Azure Data Factory (ADF)**, raw data is stored in **Azure Data Lake Storage Gen2 (ADLS Gen2)**, and data transformation and modeling are performed using **Azure Databricks and PySpark**.

The project follows the **Medallion Architecture**:

```text
Source
   │
   ▼
Azure Data Factory
   │
   ▼
🥉 Bronze Layer
   │
   ▼
Azure Databricks + PySpark
   │
   ▼
🥈 Silver Layer
   │
   ▼
Azure Databricks + PySpark
   │
   ▼
🥇 Gold Layer
   │
   ▼
Analytics / Reporting
