# automated-inventory-etl# 📦 Automated Inventory ETL & Restock Alert System

> An end-to-end data pipeline built in Microsoft Excel and Power Query to eliminate manual data entry, normalize messy stock logs, and automate inventory threshold alerts for decision-makers.

---

## 📌 The Business Challenge
In fast-paced commercial and warehouse operations, incoming stock logs are frequently received in chaotic, unstructured formats (such as raw text dumps or unformatted spreadsheets). This manual data handling causes severe bottlenecks, human errors, and a total lack of visibility over critical inventory levels—ultimately leading to costly stockouts.

## 🛠️ Tech Stack & Methodology
* **Core Tool:** Microsoft Excel
* **Data Transformation:** Power Query (M Language / ETL Pipeline)
* **Key Competencies:** Data Normalization, Schema Standardization, Conditional Business Logic, Automated Alerting.

---

## 🔄 The ETL Pipeline (Before & After)

* **1. Extract & Raw Input (`ContadorDeStockCrudo.xlsx`):**
  * Contains fragmented text strings, inconsistent date formats, and missing headers representing raw warehouse logs.
* **2. Transform & Load (`ContadorDeStock_Principal.xlsx`):**
  * **Schema Standardization:** Cleans and structures data into a production-ready format (`Product_ID`, `Product_Name`, `Entry_Date`, `Current_Stock`, `Unit_Price`).
  * **Business Logic Integration:** Implements automated conditional formatting and custom logic columns (`Restock_Status`) to instantly flag items that require immediate re-ordering.

---

## 📁 Repository Structure
```text
├── ContadorDeStockCrudo.xlsx       # Raw, unstructured source data log
├── ContadorDeStock_Principal.xlsx  # Final cleaned model with automated ETL & Restock Logic
└── README.md                       # Project documentation
