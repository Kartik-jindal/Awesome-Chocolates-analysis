# Awesome-Chocolates-analysis
# Power BI Sales Analytics Dashboard

This repository contains a **Power BI Sales Analytics Dashboard** that provides insights into sales performance, product categories, sales personnel, and regional sales distribution. The project involves data cleaning, relationship modeling, and visualization to facilitate data-driven decision-making.

## 📊 Project Overview
The dashboard integrates multiple datasets to provide a comprehensive analysis of sales data, focusing on:
- **Sales trends** over time
- **Performance of sales personnel**
- **Regional sales distribution**
- **Product-wise sales insights**

## 🗄️ Data Model
The Power BI report is built on the following dataset tables:

1. **sales**: Contains transactional sales data with fields such as `Amount`, `Boxes`, `Customers`, `Date`, `Geography`, `Product`, and `Sales Person`.
2. **products**: Holds product details, including `Category`, `Product`, and `Size`.
3. **people**: Stores information on sales personnel, including `Sales Person`, `Picture`, and `Team`.
4. **locations**: Contains geographical data with `Geo` and `Region` fields.

## 🔗 Relationships
The relationships between the tables are as follows:
- `sales(Geography)` → `locations(Geo)` (Many-to-One)
- `sales(Product)` → `products(Product)` (Many-to-One)
- `sales(Sales Person)` → `people(Sales Person)` (Many-to-One)

## 📈 Visualizations
The dashboard includes interactive visualizations such as:
- **Sales trend analysis** using line charts
- **Regional sales breakdown** using maps and bar charts
- **Top-performing sales personnel** using leaderboard-style visuals
- **Product category distribution** using pie charts and treemaps

## 🛠️ Technologies Used
- **Power BI**: Data transformation, modeling, and visualization
- **DAX (Data Analysis Expressions)**: For calculated measures and performance metrics
- **Power Query**: For data cleaning and preprocessing
