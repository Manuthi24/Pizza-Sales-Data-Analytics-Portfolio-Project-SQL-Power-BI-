
# 🍕 Pizza Sales Data Analysis Project (SQL & Power BI)
![SQL Server](https://img.shields.io/badge/SQL%20Server-SSMS%2019-red)
![T--SQL](https://img.shields.io/badge/T--SQL-KPI%20Analysis-blue)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard%20%26%20DAX-yellow)
![Data Analytics](https://img.shields.io/badge/Data-Analytics-brightgreen)
![Business Intelligence](https://img.shields.io/badge/Business-Intelligence-blueviolet)
![Excel](https://img.shields.io/badge/Excel-CSV%20Data-darkgreen)
![Portfolio Project](https://img.shields.io/badge/Type-Portfolio%20Project-important)


<p align="center">
  <img src="assests/Best Worst Sellers.jpeg" alt="Best & Worst Sellers" width="400" />
  <img src="assests/Home Dashboard.jpeg" alt="Home Dashboard" width="400" />
</p>

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
