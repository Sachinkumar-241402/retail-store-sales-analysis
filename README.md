# 🛒 Retail Store Sales Analysis

Exploratory Data Analysis (EDA) of retail store transactions using Python. 
This project cleans a raw sales dataset and uncovers sales patterns across 
product categories, locations, payment methods and time.

## 📌 Project Objective
- Clean messy retail data (missing values, wrong data types)
- Understand which categories drive the most sales
- Compare sales across Online vs In-store
- Analyse yearly and monthly sales trends
- Study relationship between price, quantity and total spent

## 📂 Dataset
- **File:** `retail_store_sales.csv`
- **Rows:** 12,575 (before cleaning) → 11,971 (after cleaning)
- **Period:** 2022 – 2025
- **Source:** (yahan Kaggle / jahan se dataset liya uska link daalo)

| Column | Description |
|---|---|
| Transaction ID | Unique ID of each transaction |
| Customer ID | Unique customer identifier |
| Category | Product category (8 categories, e.g. Food, Beverages, Furniture) |
| Item | Item name |
| Price Per Unit | Price of one unit |
| Quantity | Units purchased |
| Total Spent | Total transaction amount |
| Payment Method | Mode of payment |
| Location | Online / In-store |
| Transaction Date | Date of purchase |
| Discount Applied | Whether discount was applied |

## 🧹 Data Cleaning Steps
1. Checked missing values using `isnull().sum()`
2. Converted `Transaction Date` to datetime format
3. Dropped `Item` and `Discount Applied` columns (too many missing values)
4. Filled missing `Price Per Unit` using `Total Spent / Quantity`
5. Removed 604 rows where both `Quantity` and `Total Spent` were missing
6. Final dataset: **11,971 rows × 9 columns**

## 📊 Analysis & Visualizations
- Product category distribution (Pie chart)
- Average and total spent by category (Bar + Line chart)
- Payment method-wise spending (Pie chart)
- Year-wise total and average spent trend (Line chart)
- Location-wise sales by year (Bar chart)
- Monthly sales trend by year (Line chart)
- Distribution of Total Spent (Histogram)
- Quantity vs Total Spent, Price vs Total Spent (Scatter plots)

## 🔍 Key Insights
> (Apne charts dekh kar 4–6 points yahan likho. Example:)
- Category X had the highest total sales...
- Sales were highest in month ___ ...
- Online and In-store sales are almost equal (~6,068 vs ~5,903 transactions)...
- Payment method ___ contributed the most revenue...

## 🛠️ Tools & Libraries
- Python 3
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
