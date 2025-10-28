# 📊 Sales Trend Analysis Using Aggregations (SQL Project)

## 🧭 Overview
This project focuses on analyzing **monthly sales revenue** and **order volume** using SQL aggregation techniques.  
It helps to identify sales trends over time and gain insights into business performance.

---

## 🎯 Objective
Analyze monthly revenue and order volume from the `online_sales` dataset using SQL functions such as:
- `SUM()` for total revenue
- `COUNT()` for total orders
- `EXTRACT()` for month and year extraction
- `GROUP BY` for monthly grouping
- `ORDER BY` for sorting

---

## 🧰 Tools Used
- **MySQL / PostgreSQL / SQLite**
- SQL Editor or VS Code SQL Extension

---

## 🗃️ Dataset
**Table Name:** `online_sales`

| Column Name | Data Type | Description |
|--------------|------------|-------------|
| order_id | INT | Unique order ID |
| order_date | DATE | Date of order |
| amount | DECIMAL(10,2) | Order amount (revenue) |
| product_id | INT | Product identifier |

---

## 🧩 SQL Script

### Step 1: Create the Table
```sql
CREATE TABLE online_sales (
    order_id INT PRIMARY KEY,
    order_date DATE,
    amount DECIMAL(10,2),
    product_id INT
);
