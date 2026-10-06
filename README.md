# Azure Retail Data Engineering Platform

## Project Overview
This project is an end-to-end Azure Data Engineering solution designed to process, transform, and analyze retail e-commerce data. It ingests raw transaction data, processes it through a Medallion Architecture (Bronze, Silver, Gold), and prepares it for business intelligence reporting.

## Business Problem
RetailMart (based on the real-world Olist Brazilian E-Commerce dataset) needs a unified data platform to analyze sales performance, customer behavior, and delivery logistics. The existing data is highly relational but scattered across multiple raw CSV extracts.

## Architecture & Tech Stack
* **Data Lake:** Azure Data Lake Storage (ADLS Gen2)
* **Orchestration:** Azure Data Factory (ADF)
* **Data Processing:** Azure Databricks (PySpark)
* **Architecture Pattern:** Medallion Architecture (Bronze -> Silver -> Gold)
* **Analytics/Serving:** Azure SQL / Power BI

## Dataset
The dataset utilized is a sample of the [Olist E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce), containing anonymized information about orders, customers, products, payments, and reviews.

*(Project currently under active development)*
