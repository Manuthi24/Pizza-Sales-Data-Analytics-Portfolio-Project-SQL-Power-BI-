# 🍕 Pizza Sales Data Analysis Project (SQL & Power BI)

## 📌 Project Overview
This is an **end-to-end Data Analyst portfolio project** that demonstrates strong skills in **SQL**, **Power BI**, and **data-driven decision making**.

The project analyzes a **full year of pizza sales data (2015)** to uncover meaningful business insights for a restaurant owner.  
A **two-way validation approach** was applied by comparing SQL query outputs with Power BI DAX measures to ensure **100% KPI accuracy**.

---

## 🎯 Business Problem
The client wanted a clear understanding of sales performance in order to:
- Track business KPIs
- Identify sales trends
- Understand customer preferences
- Detect best- and worst-performing pizzas

---

## 📊 Requirements

### 🔹 KPI Requirements
- 💰 Total Revenue  
- 📦 Total Orders  
- 🍕 Total Pizzas Sold  
- 📊 Average Order Value  
- ➗ Average Pizzas per Order  

### 🔹 Visualization Requirements
- 📅 Daily Order Trends  
- 🗓️ Monthly Order Trends  
- 🍕 Sales % by Pizza Category  
- 📏 Sales % by Pizza Size  
- 🏆 Top 5 Best-Selling Pizzas  
- ⚠️ Bottom 5 Worst-Selling Pizzas  

---

## 🛠️ Tools & Technologies Used
- 🗄️ **MS SQL Server Management Studio (SSMS v19.0)**  
  - Database creation  
  - Data import  
  - KPI & trend analysis using SQL  

- 📊 **Power BI Desktop (June 2023)**  
  - Data cleaning (Power Query)  
  - DAX calculations  
  - Interactive dashboard design  

- 📁 **Excel / CSV**  
  - Raw dataset (~48,000 rows, 12 columns)

---

## 🧹 Data Cleaning & Preparation

### 🗃️ SQL Database Setup
- Created a database named **`Pizza_DB`**
- Imported raw CSV data as a flat file
- Manually corrected data types:
  - `order_id` → `INT`
  - `quantity` → `INT`
  - `total_price` → `FLOAT`
  - `pizza_name` → `VARCHAR(50)`

---

## 🔍 SQL Analysis

### 📌 Key SQL Queries

#### 💰 Total Revenue
```sql
SELECT SUM(total_price) AS Total_Revenue
FROM pizza_sales;
