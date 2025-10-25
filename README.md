# 📊 Online Retail EDA Project (Python | Pandas | Matplotlib | Seaborn | Data Analysis)

## 🧭 Project Overview
This project presents an **end-to-end Exploratory Data Analysis (EDA)** on the **Online Retail II Dataset** using **Python and Google Colab**.  
The analysis covers **data cleaning, feature engineering, visualization, and business insights** to understand sales patterns, customer behavior, and revenue trends.

---

## 🎯 Project Objectives
- Analyze customer purchase patterns and top-selling products  
- Identify outliers, missing values, and data inconsistencies  
- Explore revenue trends by time, country, and product  
- Derive actionable business insights from transaction data  

---

## 👥 Stakeholders & Key Questions

### **Stakeholders**
- **Business Manager / CEO** – Interested in overall sales performance, top products, and revenue trends.  
- **Sales & Marketing Team** – Focused on customer behavior, top buyers, and promotional opportunities.  
- **Inventory / Supply Chain Team** – Concerned with product demand, stock levels, and seasonal trends.  
- **Data Analyst / Data Science Team** – Ensures data quality and prepares features for reporting or predictive models.  

### **Stakeholder Questions**
| Stakeholder | Key Questions |
|------------|---------------|
| **Business Manager / CEO** | Which products and customers drive the most revenue? Are sales growing over time? |
| **Sales & Marketing Team** | Who are the top customers? How do sales vary across countries and seasons? Which products to promote? |
| **Inventory / Supply Chain Team** | Which products sell the most? Are there seasonal peaks in demand? Are there unusual stock movements (negative quantities/returns)? |
| **Data Analyst / Data Science Team** | Are there missing or inconsistent entries? Which outliers need treatment? How can we engineer features for better analysis? |

---

## 📊 EDA Questions

1. How are the `Quantity` values distributed? Are there negative or extremely high quantities?  
2. What is the distribution of `UnitPrice`? Which products generate the highest revenue (`Quantity × UnitPrice`)?  
3. How many unique customers are there? Who are the top customers by total purchases?  
4. Which `StockCode` or `Description` products are sold the most?  
5. How does sales vary across different countries? Which countries contribute the most to revenue?  
6. Are there seasonal trends in sales? How does `InvoiceDate` affect sales (monthly or daily patterns)?  
7. Are there missing values or unusual entries that could affect analysis, such as `CustomerID = Guest` or negative `Quantity`?  

---

## 🧮 Dataset Information
| Feature | Description |
|----------|-------------|
| **Invoice** | Invoice number of each transaction |
| **StockCode** | Product (item) code |
| **Description** | Product name or item description |
| **Quantity** | Number of items purchased (may include returns if negative) |
| **InvoiceDate** | Date and time of transaction |
| **UnitPrice** | Price per unit of product |
| **CustomerID** | Unique customer identifier |
| **Country** | Country where purchase was made |

📁 **Rows:** 1048575  
📊 **Columns:** 8  
📚 **Source:** [UCI Machine Learning Repository – Online Retail II Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail+ii)

---

## ⚙️ Tools & Libraries Used
- **Python 3**
- **Google Colab**
- **pandas** – data wrangling  
- **numpy** – numerical operations  
- **matplotlib & seaborn** – data visualization  
- **datetime** – date-time feature extraction  

---

## 🧩 Project Steps
| Step | Description |
|------|--------------|
| **1. Project Setup** | Created folders, virtual environment, and installed dependencies |
| **2. Data Understanding** | Inspected dataset shape, datatypes, and missing values |
| **3. Data Cleaning** | Filled missing values, removed duplicates, fixed data types |
| **4. EDA Questions** | Framed analytical questions from stakeholder perspective |
| **5. Univariate Analysis** | Distribution plots for numeric & categorical features |
| **6. Bivariate Analysis** | Correlation, scatterplots, and comparisons |
| **7. Feature Relationships** | GroupBy aggregations, correlation matrix, pairplots |
| **8. Outlier Detection & Treatment** | Removed negative quantities & extreme prices |
| **9. Feature Engineering** | Created Revenue, MonthYear, Weekday, Quantity bins |
| **10. Visualization Summary** | Built comprehensive dashboards & summary charts |
| **11. Insights & Conclusions** | Business insights & patterns identified |
| **12. GitHub Preparation** | Cleaned notebook, added markdowns, created README |

---

## 📈 Key Insights & Findings

- 💰 **Revenue Analysis:** Total revenue dominated by the UK, with seasonal spikes in November–December.  
- 📦 **Product Performance:** A few top products contribute the majority of total sales.  
- 👥 **Customer Behavior:** Repeat customers drive high revenue; guests are significant but untapped.  
- 🌍 **Country Trends:** UK dominates; Germany and France show growth potential.  
- 📆 **Time Patterns:** Peak sales occur in Q4; weekday and hour patterns align with shopping behavior.  
- ⚠️ **Data Quality:** Negative quantities and missing CustomerIDs were handled; duplicates removed.

---

## 🧠 Insights & Conclusions

- Strong overall sales performance with **high-revenue products** and **top customers** identified.  
- Seasonal trends suggest **holiday-focused marketing**.  
- Opportunity to **convert guest users to registered customers** for loyalty.  
- Focus on **inventory optimization** and top-performing products.  
- Dataset cleaning and feature engineering ensure reliable analysis for business decisions.

---

## 📊 Sample Visualizations
- Histogram / Boxplot → Quantity & UnitPrice distributions  
- Correlation Heatmap → Numeric feature relationships  
- Top Products Barplot → Top 10 products by revenue  
- Country-wise Revenue Chart → Country performance  
- Monthly Revenue Trend → Seasonal trends  
- Pairplot → Quantity, UnitPrice, Revenue relationships  

<img width="1302" height="556" alt="download" src="https://github.com/user-attachments/assets/ed661811-1792-4c0e-959f-2ba1e5e45585" />


---

## 🛠️ How to Run the Project
1. Open `Online_Retail_EDA.ipynb` in **Google Colab**.  
2. Upload the dataset file (`online_retail_ii_UCI_data_set.csv`).  
3. Run all cells sequentially.  
4. Cleaned dataset will be saved as `online_retail_cleaned.csv`.  

---

## 👨‍💻 Author
**Your Name**  
Data Analyst | Python | Power BI | Excel | SQL  
📧 your.email@example.com  
🔗 [LinkedIn](https://linkedin.com/in/yourprofile)  
🔗 [GitHub](https://github.com/yourusername)

---

⭐ **If you found this project insightful, don’t forget to give it a star!** ⭐
