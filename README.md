# 🛒 Grocery Sales Analysis — README

## 📌 Project Overview

This project explores a large grocery sales dataset using Python and Pandas to uncover insights that help understand product performance, customer behavior, and overall business trends.

The analysis includes:

* Data cleaning
* Exploratory Data Analysis (EDA)
* Aggregations and KPIs
* Visualizations
* Business insights

All analysis is performed inside a Kaggle Notebook using a publicly available dataset.

---

## 📂 Notebook Link

You can view and run the full notebook here:

👉 **Kaggle Notebook:**
[https://www.kaggle.com/code/naziruai/grocery-sales-analysis-2](https://www.kaggle.com/code/naziruai/grocery-sales-analysis-2)

---

# 📦 Dataset

This project uses the **Grocery Sales Dataset** on Kaggle:

🔗 **Dataset URL:**
[https://www.kaggle.com/datasets/andrexibiza/grocery-sales-dataset](https://www.kaggle.com/datasets/andrexibiza/grocery-sales-dataset)

The dataset contains multiple CSV files:

* `sales.csv`
* `products.csv`
* `customers.csv`
* `categories.csv`
* `cities.csv`
* `countries.csv`

---

# ▶️ How to Run This Notebook on Kaggle (Recommended)

Running this project on Kaggle is the easiest method because:

✔️ No installation needed
✔️ Dataset can be attached automatically
✔️ Notebook runs in the cloud

### **Steps:**

1. Open the notebook:
   👉 [https://www.kaggle.com/code/naziruai/grocery-sales-analysis-2](https://www.kaggle.com/code/naziruai/grocery-sales-analysis-2)

2. Click **Copy & Edit** (top-right corner)

3. On the right panel, click **Add Data**

4. Search for this dataset:
   `grocery-sales-dataset`

5. Select it → Click **Add**

6. Run all cells in the notebook (**Runtime → Run all**)

🎉 **Everything will work automatically — no downloads needed.**

---

# 💻 How to Run Locally (Optional)

If the user wants to run locally instead of Kaggle:

### 1. Clone or download this notebook

### 2. Install dependencies

```
pip install pandas numpy matplotlib seaborn
```

### 3. Download dataset manually

From: [https://www.kaggle.com/datasets/andrexibiza/grocery-sales-dataset](https://www.kaggle.com/datasets/andrexibiza/grocery-sales-dataset)

Place all CSV files in a `data/` folder.

### 4. Update paths in the notebook

Change lines like:

```python
sales = pd.read_csv("/kaggle/input/grocery-sales-dataset/sales.csv")
```

to:

```python
sales = pd.read_csv("data/sales.csv")
```

Run the notebook normally.

---

# 🧹 Data Cleaning Performed

* Handled missing values in categorical and numeric columns
* Combined multiple CSV files using efficient merging
* Created a sampled version of the large dataset for faster analysis
* Converted date columns to datetime for time-series analysis

---

# 📊 Analysis Performed

* Total sales calculations
* Best-selling products
* Best-performing categories
* Monthly sales trends
* Customer purchase patterns
* City & country performance

---

# 📈 Visualizations

The notebook includes:

* Line chart of monthly sales
* Bar charts for product and category ranking
* Customer distribution plots
* Time-series summaries

All visualizations are generated using Matplotlib and Seaborn.

---

# 🧠 Key Insights

Examples of insights generated:

* **Total Sales:** Computed from `Total` column
* **Best-Selling Product:** Based on highest revenue
* **Top Category:** Category with strongest performance
* **Peak Sales Month:** Determined from grouped monthly totals

---

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

# 📫 Contact

* LinkedIn
* GitHub
* Email

---

# 📜 License

MIT License © 2025 NaziruAI

---
