# End-to-End-Data-Engineering-Pipeline

## Overview

This project implements an end-to-end data pipeline using the Medallion Architecture (Bronze, Silver, Gold) on the Olist dataset (Kaggle).

Data is ingested from Azure Data Lake Storage into the Lakehouse using pipelines, then processed with PySpark (Fabric Notebooks) to produce analytics-ready datasets.

---

## Architecture

* **Bronze**: Raw data ingested via pipeline, then converted to Delta tables with schema enforcement
* **Silver**: Data cleaning, standardization, and transformations
* **Gold**: Business-ready tables using star schema

---

## Pipeline

Orchestrated using Microsoft Fabric Pipelines:

* Copy Activity → Ingest raw data from ADLS to Lakehouse
* Bronze Notebook → Apply schema and convert data to Delta tables
* Silver Notebook → Clean and transform data
* Gold Notebook → Aggregate and model data

---

## Processing

* PySpark (Fabric Notebooks)
* Delta Lake
* Layered processing (Bronze → Silver → Gold)

---


## Dataset

Olist dataset from Kaggle:
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce


---


