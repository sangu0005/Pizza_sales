# 🍕 Pizza Sales Analysis – SQL + Power BI Dashboard  

🚀 **Data-driven insights** into pizza sales using SQL & Power BI – uncovering trends, top performers, and revenue drivers to help optimize business decisions.  

---

## 📊 **Project Overview**  
This project explores **pizza sales data** using SQL for data extraction and Power BI for visualization.  
The dashboard highlights **revenue trends, best/worst sellers, and sales distribution by category & size**.

---

## 🛠️ **Tech Stack**
- 🗄 **SQL** – KPI calculations, trend analysis  
- 📊 **Power BI** – Interactive dashboard creation  
- 📂 **Dataset** – Pizza sales (orders, categories, quantities, prices)

---

## 🧮 **Key SQL Queries**

🔑 **KPI Metrics**
```sql
-- Total Revenue
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;

-- Average Order Value
SELECT (SUM(total_price) / COUNT(DISTINCT order_id)) AS Avg_order_Value
FROM pizza_sales;

-- Total Pizzas Sold
SELECT SUM(quantity) AS Total_pizza_sold FROM pizza_sales;
