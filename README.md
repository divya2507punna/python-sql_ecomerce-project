# 📊 E-commerce Data Analysis with MySQL & Python

## 📌 Project Overview
This project explores a large-scale E-commerce dataset using Python and MySQL to extract valuable business insights. The dataset includes customer transactions, order details, seller information, payments, and product details.

I built a structured data pipeline that involves:
- **Data Cleaning & Preprocessing** – Handling missing values, formatting data
- **Database Integration** – Storing structured data in MySQL
- **Data Analysis & Visualization** – Identifying trends and customer behaviors
- **Query Optimization** – Enhancing SQL queries for faster analysis

This project helps businesses understand customer purchasing behavior, sales trends, and revenue distribution across product categories.

## 🚀 Technologies Used
- **Python** – Pandas, NumPy, Seaborn, Matplotlib, MySQL Connector
- **MySQL** – Data Storage, Query Execution
- **Jupyter Notebook** – Interactive Analysis
- **GitHub** – Version Control
- **MySQL Workbench** – Database Management

## 🚀 What I Built & My Key Contributions
### ✅ Automated Data Loading & Processing
- Developed a Python script to automate data ingestion from CSV files into MySQL.
- Used Pandas to handle missing values and clean column names.
- Designed an intelligent schema detection system that maps CSV column types to MySQL data types dynamically.

### ✅ Optimized MySQL Queries
- Wrote efficient SQL queries to extract key insights like customer distribution, sales trends, and payment behaviors.
- Used JOIN operations to connect multiple tables efficiently.
- Applied window functions for advanced analytics, such as cumulative revenue tracking and customer retention rates.

### ✅ Interactive Data Visualization
- Utilized Matplotlib & Seaborn to create bar charts, histograms, and correlation heatmaps.
- Plotted sales trends over time to help businesses identify high-performing months.

### ✅ Customer & Seller Insights
- Analyzed customer locations to understand geographic trends.
- Ranked sellers by revenue to determine top-performing vendors.

## 💡 Challenges Faced & How I Overcame Them
### 1️⃣ Handling Missing Data
**📌 Challenge:** Some datasets (e.g., products.csv) had missing product categories, prices, and descriptions.

**💡 Solution:** Used Pandas `.fillna()` to fill missing values and converted categorical missing data into "Unknown" for better handling.

```python
df["product_category"] = df["product_category"].fillna("Unknown")
df.fillna(0, inplace=True)  # Replace NaN with 0 for numerical columns
