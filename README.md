## [md](https://github.com/renuka12294/Vendor-performance-analysis/tree/main/Vendor-Performance-analysis-main/Vendor-Performance-analysis-main#readme)

# 📊 Vendor Performance Analysis -- Retail Inventory & Sales Dashboard

Analyzing vendor performance, sales, inventory, and profitability using **MySQL, SQL, Python, and Power BI**.

---

# 📌 Table of Contents

- Overview
- Business Problem
- Dataset
- Tools & Technologies
- Project Structure
- Data Cleaning & Preparation
- Exploratory Data Analysis (EDA)
- Research Questions & Key Findings
- Power BI Dashboard
- How to Run
- Business Recommendations
- Author

---

# 📖 Overview

This project analyzes retail inventory and vendor performance by combining purchase, sales, inventory, and vendor invoice data into a centralized analytical dataset. The objective is to generate business insights that support purchasing, inventory optimization, and vendor evaluation.

---

# 💼 Business Problem

The project answers important business questions such as:

- Which vendors generate the highest sales?
- Which vendors contribute the most to purchases?
- Which vendors have low inventory turnover?
- Which brands need promotional or pricing adjustments?

---

# 📂 Dataset

The project uses six source tables:

- Purchases
- Sales
- Purchase Prices
- Vendor Invoice
- Beginning Inventory
- Ending Inventory

A consolidated table named **vendor_sales_summary** was created using SQL joins and aggregations for analysis and dashboard creation.

---

# 🛠 Tools & Technologies

### Languages

- Python
- SQL

### Database

- MySQL
- MySQL Workbench

### Python Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- SQLAlchemy
- PyMySQL

### Business Intelligence

- Microsoft Power BI Desktop

### Development Environment

- Jupyter Notebook
- MySQL Workbench
- Power BI

---

# 📁 Project Structure

```
Vendor-Performance-Analysis/
│
├── README.md
├── notebooks/
│   ├── Data_Cleaning.ipynb
│   ├── Exploratory_Data_Analysis.ipynb
│   └── Vendor_Performance_Analysis.ipynb
│
├── sql/
│   ├── create_vendor_sales_summary.sql
│   └── analytical_queries.sql
│
├── dashboard/
│   └── Vendor_Performance_Dashboard.pbix
│
└── screenshots/
    └── dashboard.png

```

---

# 🔄 Data Pipeline

```
CSV Files
     │
     ▼
MySQL Database
     │
     ▼
SQL Joins & Aggregations
     │
     ▼
vendor_sales_summary
     │
     ▼
Python (EDA & Cleaning)
     │
     ▼
Power BI Dashboard

```

---

# 🧹 Data Cleaning & Preparation

Performed the following steps:

- Imported CSV files into MySQL
- Created relational tables
- Joined multiple tables using SQL
- Created `vendor_sales_summary`
- Converted data types
- Removed missing values
- Removed records with:
  - GrossProfit ≤ 0
  - ProfitMargin ≤ 0
  - TotalSalesQuantity ≤ 0
- Calculated:
  - Gross Profit
  - Profit Margin
  - Stock Turnover
  - Sales to Purchase Ratio

---

# 📊 Exploratory Data Analysis (EDA)

Performed:

- Histograms
- Box Plots
- Count Plots
- Correlation Heatmap
- Vendor Analysis
- Brand Analysis
- Purchase Contribution Analysis
- Stock Turnover Analysis

---

# ❓ Research Questions & Key Findings

### 1. Which vendors generate the highest sales?

Top 10 vendors were identified using TotalSalesDollars.

### 2. Which brands need promotional or pricing adjustments?

Brands with low sales but high profit margins were identified for promotion.

### 3. Which vendors contribute the most to purchases?

Purchase contribution percentages were calculated for each vendor.

### 4. Which vendors have low inventory turnover?

Vendors with StockTurnover < 1 were identified as holding slow-moving inventory.

### 5. How profitable are vendors?

Gross Profit and Profit Margin were analyzed to evaluate vendor performance.

---

# ▶ How to Run This Project

1. Import datasets into MySQL.
2. Execute SQL queries to create `vendor_sales_summary`.
3. Run Python notebooks for cleaning and EDA.
4. Connect Power BI to MySQL.
5. Load `vendor_sales_summary`.
6. Build or refresh the dashboard.

---

# 💡 Business Recommendations

- Increase promotions for high-margin, low-selling brands.
- Reduce dependency on a few vendors.
- Improve inventory turnover.
- Optimize purchasing strategies.
- Monitor vendor performance regularly.

---

# 👨‍💻 Author

# Renuka

**B.E. Information Science & Engineering**

### Skills

- Python
- MySQ
- SQL
- Microsoft Excel
- Power BI
- Data Analytics
- Data Visualization
