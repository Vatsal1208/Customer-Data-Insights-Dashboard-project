# 📊 Customer Data Insights Dashboard

A Python-based data analysis project that processes e-commerce customer and sales data, performs analysis using **Pandas** and **NumPy**, and visualizes insights with **Matplotlib**. Built using Object-Oriented Programming (OOP) principles.

---

## 📁 Project Structure
```
customer_data_insights/
│
├── datasets/
|   ├── combined.csv
│   ├── List of Orders.csv
│   ├── Order Details.csv
│   └── Sales target.csv
│
├── sql_csv_findings/
│   ├── sql_category_sales.csv
│   ├── sql_monthly_sales.csv
│   └── sql_top_customers.csv
│
├── visualization_chart/
│   ├── chart_1_top_products.png
│   ├── chart_2_category_pie.png
│   └── chart_3_monthly_trend.png
│
├── customer_data.ipynb
├── customer_data_insights.ipynb
├── summary_results.csv
└── README.md
```
---

## Getting Started

### Prerequisites

Make sure you have Python installed along with the following libraries:

```bash
pip install pandas numpy matplotlib
```

For the optional SQL extension:

```bash
pip install mysql-connector-python
```

### Running the Project

1. **Clone the repository**

   ```bash
   git clone https://github.com/Vatsal1208/customer-data-insights.git
   cd customer-data-insights
   ```
2. **Open the notebooks in order:**

   - Start with `customer_data.ipynb` — loads and merges the raw CSV files, saves `combined.csv`
   - Then run `customer_data_insights.ipynb` — performs full analysis and generates charts
3. **Update file paths** in `customer_data.ipynb` to match your local system:

   ```python
   orders_csv = "datasets/List of Orders.csv"
   order_details_csv = "datasets/Order Details.csv"
   sales_target_csv = "datasets/Sales target.csv"
   ```

---

## 📌 Features

| Feature                             | Status                     |
| ----------------------------------- | -------------------------- |
| Data Loading (CSV)                  | ✅ Implemented             |
| Data Cleaning                       | ✅ Implemented             |
| OOP —`CustomerData` class        | ✅ Implemented             |
| Data Analysis (Pandas + NumPy)      | ✅ Implemented             |
| Data Visualization (bar, pie, line) | ✅ Implemented             |
| File Export (CSV + PNG)             | ✅ Implemented             |
| SQL Operations                      | ⭐ Optional — implemented |

### ✅ Data Cleaning

- Removes duplicate records
- Handles missing values
- Converts `Order Date` to datetime format
- Extracts `Month` column for time-series analysis

### ✅ OOP Design — `CustomerData` Class

| Method                       | Description                                |
| ---------------------------- | ------------------------------------------ |
| `__init__(dataframe)`      | Initializes with a cleaned dataframe       |
| `clean_data()`             | Deduplicates, handles nulls, formats dates |
| `analyze()`                | Runs full analysis and prints results      |
| `export_results(filename)` | Saves summary to CSV                       |

---

## 📊 Key Findings

### Metrics

| Metric              | Value                |
| ------------------- | -------------------- |
| Total Customers     | 332 unique customers |
| Total Sales         | ₹4,31,502           |
| Total Orders        | 500 orders           |
| Average Order Value | ₹863                |

### Top 5 Customers by Purchase Amount

1. Yaanvi — ₹9,177
2. Pooja — ₹9,030
3. Abhishek — ₹8,135
4. Surabhi — ₹6,889
5. Soumya — ₹6,869

### Top 5 Best-Selling Products

1. Printers — ₹58,252
2. Bookcases — ₹56,861
3. Saree — ₹53,511
4. Phones — ₹46,119
5. Electronic Games — ₹39,168

### Category Analysis

| Category    | Revenue    | Share |
| ----------- | ---------- | ----- |
| Electronics | ₹1,65,267 | 38.3% |
| Clothing    | ₹1,39,054 | 32.2% |
| Furniture   | ₹1,27,181 | 29.5% |

> **Key Insight:** Electronics is the dominant category with the highest revenue at 38.3% of total sales.

### Sales Trends

- 📈 **Peak Month:** January 2019 — ₹61,439
- 📉 **Lowest Month:** July 2018 — ₹12,966
- 📊 **Average Monthly Sales:** ₹35,958

### NumPy Stats Analysis

| Stat          | Value                                    |
| ------------- | ---------------------------------------- |
| Mean          | ₹287.67 per transaction                 |
| Median        | ₹118.00                                 |
| Std Deviation | ₹460.90 (high variance in order values) |
| Price Range   | ₹4 — ₹5,729                           |

---

## 📝 Conclusion

This analysis provides valuable insights into customer behavior, product performance, and sales trends. Electronics leads all categories at 38.3% of total revenue, Printers and Bookcases are the top-selling products, and sales peaked in January 2019 with consistent growth in early 2019.

---

## 🛠️ Technologies Used

| Tool             | Purpose                          |
| ---------------- | -------------------------------- |
| Python 3         | Core language                    |
| Pandas           | Data loading, cleaning, analysis |
| NumPy            | Statistical calculations         |
| Matplotlib       | Data visualization               |
| Jupyter Notebook | Interactive development          |
| MySQL (optional) | SQL storage and queries          |

---

## 👤 Author

**Vatsal**
Mini Project — November 2025
Python Data Analysis | Pandas | NumPy | Matplotlib
