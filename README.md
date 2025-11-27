# 🛒 Grocery Sales Analysis

*A Complete Data Cleaning, Merging, and Exploratory Data Analysis (EDA) Project*

## 📌 Overview

This notebook performs a complete end-to-end analysis of a large grocery sales dataset from Kaggle.
The goal is to understand product performance, customer behavior, category sales trends, and overall business insights.

The notebook covers:

* Dataset loading
* Efficient sampling (because full dataset > 6M rows)
* Merging multiple related CSV files
* Data cleaning and handling missing values
* Feature engineering
* Exploratory Data Analysis (EDA)
* Visualizations
* Key insights for business decision-making

---

## 📁 Dataset Description

The original Kaggle dataset contains several relational tables:

* **sales.csv** – Transaction-level sales data
* **products.csv** – Product details
* **customers.csv** – Customer demographics
* **categories.csv** – Product categories
* **cities.csv** – Cities of customers
* **countries.csv** – Country information

Because the dataset is huge, the notebook includes **sampling** to 100k rows for easier processing on Kaggle.

---

## ⚙️ Steps Performed in the Notebook

### 1️⃣ Load Datasets

Each CSV file is loaded into a separate DataFrame.

### 2️⃣ Sample the Sales Data

To avoid RAM crash or long merging time, the notebook samples:

```python
sales_sample = sales.sample(n=100_000, random_state=42)
```

### 3️⃣ Merge All DataFrames

A full merged dataset is created using:

* ProductID → products
* CustomerID → customers
* CategoryID → categories
* CityID → cities
* CountryID → countries

### 4️⃣ Handle Missing Values

Columns with <2% missing values (e.g., **MiddleInitial**, **SalesDate**) were imputed appropriately using:

* Mode for categorical
* Forward/Backward fill for dates

### 5️⃣ Feature Engineering

New useful columns:

* **Total = Quantity × UnitPrice**
* **Month extracted** from SalesDate

### 6️⃣ Exploratory Data Analysis

The notebook analyzes:

* Total revenue
* Best-selling products
* Most profitable categories
* Monthly trends
* Customer purchasing patterns

### 7️⃣ Visualizations

Charts generated include:

* 📈 Monthly Sales Trend (line plot)
* 📊 Product Sales Ranking (bar chart)
* 🍞 Category Revenue Comparison
* 👥 Customer Demographics

---

## 📊 Key Insights

```python
print("📊 KEY INSIGHTS")
print("- Total Sales:", merged_df['Total'].sum())
print("- Best Selling Product:", top_products.index[0])
print("- Best Category:", category_sales.index[0])
print("- Month with Highest Sales:", merged_df.groupby('Month')['Total'].sum().idxmax())
```

Summary:

* **Total Sales:** Total revenue generated
* **Best Selling Product:** Most purchased product
* **Top Category:** Category generating the highest revenue
* **Peak Month:** The month with highest sales volume

---

## 🧠 What I Learned

* How to merge large relational datasets efficiently
* How to sample large data to avoid RAM crash
* How to clean and transform mixed data types
* How to perform real-world EDA
* How to visualize sales trends and business patterns
* How to produce actionable insights from raw data

---

## 👨‍💻 Author

**Naziru Abdussalam Ibrahim**
A passionate Data Science & AI enthusiast from Kano, Nigeria.
Loves working on practical analytics and real-world datasets.

📫 Contact: *LinkedIn | GitHub | Email*

---

## 🏁 Conclusion

This notebook demonstrates how data analysis can help grocery businesses:

* Track product performance
* Understand seasonality
* Improve inventory decisions
* Increase revenue through better insights

It serves as a strong portfolio project showing my ability to work with **large datasets**, **data cleaning**, **EDA**, and **visualization**.

feel free to explore the notebook and reach out for any questions or collaborations!
