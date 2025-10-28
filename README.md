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

### Step 2: Inserting sample data
```sql
INSERT INTO online_sales (order_id, order_date, amount, product_id) VALUES
(1, '2024-01-15', 250.00, 101),
(2, '2024-01-28', 180.00, 102),
(3, '2024-02-10', 300.00, 103),
(4, '2024-02-22', 150.00, 104),
(5, '2024-03-05', 400.00, 101),
(6, '2024-03-18', 220.00, 102),
(7, '2024-04-01', 500.00, 103),
(8, '2024-04-20', 350.00, 104);
