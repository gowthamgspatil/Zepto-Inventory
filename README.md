# Zepto-Inventory

Based on your notebook (`Zepto_Inventory_Dataset_Insights.ipynb`), the uploaded Excel file (`zepto_v1.xlsx`), and the visualizations, here is a complete and well-structured `README.md` for your **Zepto Inventory Discount Analysis** project:

---

# 📊 Zepto Inventory Discount Analysis

This project explores the **discount strategies and pricing trends** of Zepto's product inventory dataset. It uses Python for data preprocessing, analysis, and visualization. The analysis focuses on how discounts vary across product categories, price levels, and available stock.

---

## 🔍 Objectives

* Analyze product discount patterns
* Visualize the relationship between discount percent, price, and quantity
* Understand category-wise discount trends
* Identify products with high or low discounts

---

## 📁 Dataset

**File**: `zepto_v1.xlsx`
**Source**: Zepto Inventory Data (self-curated/simulated)
**Key Columns**:

* `product name`
* `category`
* `mrp` (Maximum Retail Price)
* `selling_price`
* `available_stock`

---

## 🧮 Key Metrics Derived

New columns generated during data cleaning and feature engineering:

* **discount\_amount** = `mrp - selling_price`
* **discount\_percent** = `(discount_amount / mrp) * 100`
* **discounted\_price** = `selling_price`

---

## 📊 Visualizations & Insights

### 1. Bubble Chart: Discount % vs Price vs Stock

![Bubble Chart](./bubble_discount_vs_price.png)

* **X-axis**: Discount Percent
* **Y-axis**: Discounted Selling Price
* **Bubble Size**: Available Quantity

**Insight**:
Most products are priced under ₹60,000 with low discount percentages (< 10%). A few outliers have discounts above 30% and high MRP, indicating premium or overstocked products.

---

### 2. Line Chart: Sorted Discount Trend

![Line Chart](./line_discount_trend.png)

* **X-axis**: Product Index (sorted)
* **Y-axis**: Discount Percent

**Insight**:
Very few products receive > 30% discount. A majority cluster between 0–10%, showing a conservative pricing strategy.

---

### 3. Violin Plot: Discount Distribution by Category

![Violin Plot](./violin_discount_by_category.png)

**Insight**:

* **Fruits & Vegetables** tend to have slightly higher and more consistent discounts.
* Most categories have discounts centered around 0–10%, indicating limited seasonal offers or price cuts.
* Some outliers indicate high discounting strategies for clearance or promotion.

---

## 🛠️ Tools Used

* **Python**: `pandas`, `matplotlib`, `seaborn`
* **Jupyter Notebook**: For interactive analysis
* **Excel**: Original dataset
* **GitHub**: Project version control

---

## 📌 Key Findings

* Discounts are concentrated below 10% for the majority of products.
* Categories like **Fruits & Vegetables** show relatively higher average discounts.
* There’s no strong linear correlation between discount percent and selling price.
* High-priced items may receive higher discounts to drive sales.

---

## 📂 Folder Structure

```
├── zepto_v1.xlsx                      # Raw inventory data
├── Zepto_Inventory_Dataset_Insights.ipynb  # Main analysis notebook
├── bubble_discount_vs_price.png      # Bubble chart image
├── line_discount_trend.png           # Line chart image
├── violin_discount_by_category.png   # Violin plot image
└── README.md                         # Project documentation
```

---

## 📈 Future Scope

* Add **time series** trends of discount evolution
* Include **location-wise** discount analysis if data available
* Build a **dashboard** using Streamlit or Power BI for real-time exploration

---

## 🙌 Author

**Gowtham G S Patil**
*Data Analyst | Python | Excel | Visualization Enthusiast*


