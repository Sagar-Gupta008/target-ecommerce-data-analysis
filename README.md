# 🛒 Target E-Commerce Data Analysis

## 📌 Project Overview

This project analyzes a large-scale Brazilian e-commerce dataset to uncover patterns in sales, customer behavior, product performance, payments, and seller performance.

The analysis combines **Python and SQL** to explore the data from both analytical and business perspectives. Python was used for data exploration and visualization, while MySQL was used to answer business questions ranging from basic aggregations to advanced analytical queries involving CTEs and window functions.

---

## 🎯 Business Objective

The objective of this project is to transform raw e-commerce transactional data into meaningful business insights that can support data-driven decision-making.

The analysis focuses on questions such as:

- How are orders distributed across cities and states?
- Which product categories contribute the most to sales?
- How do sales and order volumes change over time?
- Which sellers and customers contribute the most revenue?
- How frequently do customers use installment payments?
- Is there a relationship between product price and purchase frequency?
- How are sales growing year over year?
- How can customers and sellers be ranked based on their performance?

---

## 📊 Dataset

The project uses the **Target Brazilian E-Commerce dataset**, containing information about customers, orders, products, sellers, payments, and geographic locations.

The relational dataset allows multiple tables to be joined using common identifiers such as customer IDs, order IDs, product IDs, and seller IDs.

The analysis covers e-commerce transactions across multiple years and geographic locations in Brazil.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **Python** | Data analysis and exploratory analysis |
| **Pandas** | Data manipulation and exploration |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical visualization |
| **MySQL** | Database querying and business analysis |
| **Jupyter Notebook** | Analysis and documentation environment |

---

## 🔄 Analysis Workflow

```text
Raw E-Commerce Data
        ↓
Data Exploration
        ↓
Python Analysis
        ↓
MySQL Database
        ↓
SQL Business Queries
        ↓
Advanced Analysis
        ↓
Business Insights
---

## 🧠 SQL Business Analysis

The SQL analysis was structured across **basic, intermediate, and advanced business questions**, progressing from aggregations and joins to analytical queries using CTEs and window functions.

### 🔹 Basic Analysis

- Identified unique customer locations across the dataset
- Analyzed order volume by year
- Calculated total sales contribution by product category
- Evaluated customer usage of installment payments
- Analyzed customer distribution across Brazilian states

### 🔹 Intermediate Analysis

- Analyzed monthly order trends
- Calculated average products ordered by customers across cities
- Evaluated revenue contribution by product category
- Examined the relationship between product price and purchase frequency
- Ranked sellers based on generated revenue

### 🔹 Advanced Analysis

- Calculated moving averages of customer order values
- Measured cumulative monthly sales
- Analyzed year-over-year sales growth
- Explored customer purchasing behavior over time
- Identified and ranked the highest-spending customers by year

### 🧩 SQL Concepts Demonstrated

`JOINs` • `GROUP BY` • `Aggregations` • `CASE WHEN` • `Subqueries` • `CTEs` • `DENSE_RANK()` • `LAG()` • `Window Functions` • `Moving Averages` • `Cumulative Analysis`

---
## 💡 Key Findings

### 📦 Order Activity
- **45,101 orders** were recorded in 2017, demonstrating substantial transaction activity during the period analyzed.

### 🛍️ Product Category Performance
- **Bed, Table & Bath** contributed approximately **10.70%** of analyzed category revenue.
- **Health & Beauty** followed at approximately **10.35%**.
- **Computer Accessories** contributed approximately **9.90%**.

These categories emerged among the strongest contributors to overall sales.

### 💳 Price vs Purchase Frequency
- The analysis produced a correlation of approximately **-0.106** between average product price and purchase frequency.
- This indicates a **very weak negative linear relationship**, suggesting that price alone was not a strong indicator of how frequently products were purchased.

### 📈 Sales Growth
- Year-over-year analysis showed approximately **20% growth in sales for 2018** compared with 2017 within the available dataset.
- Since the available 2018 records do not represent a complete calendar year, this result should be interpreted within the dataset's available time coverage.

### 🏆 Customer & Seller Performance
- Revenue-based ranking was used to identify high-performing sellers.
- Annual customer-spending analysis identified the highest-value customers using SQL window functions and ranking techniques.
