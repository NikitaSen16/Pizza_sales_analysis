# 🍕 Pizza Sales Analysis

This project analyzes a year's worth of pizza sales data to perform data cleaning, datetime processing,
and exploratory data analysis (EDA). The goal is to uncover trends in orders, revenue distribution 
across pizza types, and overall business performance.

---

## 📌 Project Objective

- Clean and preprocess raw pizza order data  
- Analyze pizza sales across time, size, and category  
- Calculate KPIs like total revenue, top-selling pizzas, and revenue drivers  
- Visualize order volumes and distribution trends  
- Identify best-performing products by order volume and revenue  

---

## 🧰 Tools & Technologies

- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  

---

## 🧹 Data Cleaning & Preprocessing

- Dropped unused column: `order_details_id`  
- Converted data types:  
  - `quantity` → `int8`  
  - `order_id` → `int16`  
  - `unit_price`, `total_price` → `float32`  
  - `order_date` → `datetime`  
- Combined `order_date` and `order_time` into `order_datetime`  
- Set `order_datetime` as the index  

---

## 📊 Exploratory Data Analysis

- 📅 **Total Revenue:** ₹8,17,860.06  
- 🏆 **Top 5 Most Ordered Pizzas:**
  - Classic Deluxe Pizza – 2,416 orders  
  - Barbecue Chicken Pizza – 2,372  
  - Hawaiian Pizza – 2,370  
  - Pepperoni Pizza – 2,369  
  - Thai Chicken Pizza – 2,315  

- 💸 **Top Revenue-Generating Pizzas:**
  - Thai Chicken Pizza – ₹43,434.25  
  - Barbecue Chicken Pizza – ₹42,758.00  
  - California Chicken Pizza – ₹41,489.50  

- 🍕 **Orders by Category:**
  - Classic – 14,579  
  - Supreme – 11,864  
  - Veggie – 11,674  
  - Chicken – 10,503  

- 📦 **Orders by Pizza Size:**
  - L – 18,737  
  - M – 15,685  
  - S – 13,881  
  - XL – 265  
  - XXL – 52  

---

## 📈 Visual Highlights

- Line plot of **daily order volume** (resampled by day)  
- Count plots: **pizza category** and **pizza size**  
- Bar chart: **Top 10 most ordered pizzas**  
- Box plots for **revenue distribution** by size and category  

---

## 📊 KPI Summary

| Metric            | Value         |
|-------------------|---------------|
| Total Revenue     | ₹8,17,860.06  |
| Most Ordered Pizza| Classic Deluxe Pizza (2,416 orders) |
| Top Revenue Pizza | Thai Chicken Pizza (₹43,434.25) |
| Avg Pizza Price   | ₹16.82        |
| Max Order Value   | ₹83.00        |

---

## 🔍 Key Insights

- Classic pizzas are most frequently ordered across all sizes  
- Large-sized (L) pizzas are the most sold by volume  
- Thai Chicken Pizza and Barbecue Chicken Pizza are top revenue contributors  
- Classic Deluxe Pizza is the most popular by order count  
- Pizza size impacts revenue more than category in some cases  
