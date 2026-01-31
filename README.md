# 🍽️ Food Delivery Data Analysis Project

This project analyzes a food delivery platform’s data by combining information from multiple data sources and generating business insights.

It was created as part of a data analytics hackathon to demonstrate skills in **data cleaning, data integration, and exploratory data analysis** using Python.

---
 Link of Jupiter Notebook - https://colab.research.google.com/drive/1kHogUVU0LIvoxVwqpKevxnpvnxtCRijh?usp=sharing
## 📂 Datasets Used

Three different datasets were provided, simulating real-world systems:

1. **orders.csv** – Transactional order data  
2. **users.json** – User master data  
3. **restaurants.sql** – Restaurant master data  

These datasets were merged to create a single analytical dataset:

📁 **final_food_delivery_dataset.csv**

---

## ⚙️ Steps Performed

### 1️⃣ Data Loading
- Loaded CSV, JSON, and SQL data into Python using **Pandas** and **SQLite**

### 2️⃣ Data Cleaning
- Checked for missing values
- Converted date columns into proper datetime format
- Verified data consistency

### 3️⃣ Data Integration
Performed **LEFT JOINS** to combine the datasets:

- `orders.user_id → users.user_id`
- `orders.restaurant_id → restaurants.restaurant_id`

This ensured all orders were retained while enriching them with user and restaurant details.

### 4️⃣ Feature Engineering
- Extracted month and quarter from order dates
- Created rating ranges for analysis
- Aggregated user and city-level metrics

### 5️⃣ Data Analysis & Business Insights

The final dataset was analyzed to answer business questions such as:

✔ Order trends over time  
✔ City-wise and cuisine-wise revenue  
✔ Gold vs Regular member behavior  
✔ Restaurant rating impact on revenue  
✔ Seasonal and quarterly revenue trends  
✔ High-value customers and spending patterns  

---

## 📊 Key Insights

- Gold members contribute significantly higher average order values
- Certain cities generate much higher loyalty-based revenue
- Cuisine preference influences order value
- Higher-rated restaurants drive strong revenue performance
- Seasonal patterns affect overall revenue distribution

---

## 🛠 Tools & Technologies

- Python 🐍  
- Pandas  
- NumPy  
- Matplotlib & Seaborn  
- SQLite  
- Jupyter Notebook  

---

## 📎 Project Files

| File | Description |
|------|-------------|
| `food_delivery_analysis.ipynb` | Full step-by-step analysis notebook |
| `final_food_delivery_dataset.csv` | Final merged dataset |
| `README.md` | Project documentation |

---

## 🚀 Conclusion

This project demonstrates how raw data from multiple sources can be transformed into actionable business insights using data analytics techniques. It showcases practical skills in data wrangling, integration, and visualization.

---

👨‍💻 Created for Data Analytics Hackathon  
