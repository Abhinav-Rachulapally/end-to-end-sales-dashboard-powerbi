# End-to-End Sales Dashboard with Power BI, dbt & Python

This project simulates an end-to-end sales reporting pipeline using Python, SQL, dbt, and Power BI — from raw data ingestion to BI dashboard delivery.

---

## 🧰 Tech Stack

- **Data Ingestion & Cleaning**: Python (Pandas)
- **Data Modeling**: dbt (modular SQL models)
- **Warehouse**: PostgreSQL (can simulate Redshift locally)
- **Reporting**: Power BI (Sales Metrics Dashboard)

---

## 🏗️ Architecture Overview
+------------------+
| sample_sales.csv |
+--------+---------+
         |
         v
+---------------------------+
| Python (Pandas Cleaning) |
+--------+------------------+
         |
         v
+---------------------------+
| Load into PostgreSQL     |
+--------+------------------+
         |
         v
+---------------------------+
| dbt (SQL Transformations)|
|  - staging models        |
|  - marts models          |
+--------+------------------+
         |
         v
+---------------------------+
| Power BI Dashboard       |
| - Trend analysis         |
| - Sales by region        |
| - Monthly performance    |
+---------------------------+

---

## 📁 Folder Structure
end-to-end-sales-dashboard-powerbi/
│
├── data/
│   ├── sample_sales.csv              ← Raw sales data (CSV)
│   └── sales_clean.csv               ← Cleaned data via Pandas
│
├── notebooks/
│   └── data_cleaning.ipynb           ← Data cleaning with Pandas
│
├── dbt/
│   ├── dbt_project.yml               ← dbt project config
│   └── models/
│       ├── staging/
│       │   └── stg_sales.sql         ← Cleansed + renamed fields
│       └── marts/
│           └── sales_summary.sql     ← Aggregated data for BI
│
├── dashboard/
│   └── sales_dashboard.png           ← Screenshot of Power BI dashboard
│
└── README.md                         ← Documentation & overview


---

## 📊 Dashboard Overview

The Power BI dashboard includes:

- Daily Sales Trends
- Product-wise Sales Breakdown
- Region/State Performance
- Sales by Salesperson
- Monthly Targets vs Actuals

> *(Image uploaded in `dashboard/sales_dashboard.png`)*

---

## 👨‍💻 Author

**Abhinav Rachulapally**  
Data Engineer | ETL & BI | dbt | Power BI  
[GitHub Profile](https://github.com/abhinavrachulapally)


