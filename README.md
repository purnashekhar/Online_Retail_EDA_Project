
# 📦 **Online Retail – Exploratory Data Analysis (EDA) Project**

### *(Python | Pandas | Matplotlib | Seaborn | Power BI /Data Analysis)*

---

## 🧭 **Project Objective**

The objective of this Online Retail EDA project was to analyze transactional data from an international retail store to understand:

* Overall sales performance
* Customer purchasing behavior
* Product demand patterns
* Seasonal and monthly sales trends

The project delivers insights on **top products**, **top customers**, **country-level revenue**, and **time-based demand patterns**, helping the business improve **strategic decisions**, **forecasting**, and **inventory planning**.

---

## 👥 **Stakeholder Questions**

The dataset contained **540K+ rows** and multiple features such as InvoiceNo, StockCode, Description, Quantity, UnitPrice, CustomerID, and Country.

The project answers these business-critical questions:

### **Key Business Questions**

* How are **Quantity** and **UnitPrice** distributed? Are there negative or extreme values?
* Which products generate the **highest revenue**?
* Who are the **top customers**?
* How many **unique customers** does the business have?
* Which **countries contribute** most to total revenue?
* Which **months** show the highest sales?
* Are there **seasonal or weekday** sales patterns?
* What data quality issues exist (missing IDs, negative quantity, duplicates)?
* How do sales differ across **quantity segments** (1–5, 6–20, 100+)?

---

## 🧼 **Data Cleaning & Preparation**

### ✔ **Data Cleaning Steps**

* Removed **duplicate** records
* Converted `InvoiceDate` → datetime
* Converted `CustomerID` → string
* Replaced missing CustomerIDs with `"Guest"`
* Removed invalid transactions:

  * Negative **Quantity**
  * Negative **UnitPrice**
* Cleaned Description field and replaced missing values with `"None"`

### ✔ **Feature Engineering**

New features were created for deeper analysis:

| Feature            | Description                         |
| ------------------ | ----------------------------------- |
| **Revenue**        | Quantity × UnitPrice                |
| **InvoiceYear**    | Year extracted from date            |
| **InvoiceMonth**   | Month extracted for trend analysis  |
| **MonthYear**      | Combined year–month for time-series |
| **InvoiceWeekday** | Day of week                         |
| **QuantityBin**    | 1–5, 6–20, 21–50, 51–100, 100+      |
| **TopProduct**     | High-selling product labels         |

These features support revenue segmentation, trend discovery, and customer analysis.

---

## 📊 **Data Analysis**

The analysis was performed using **Python (Pandas, NumPy)** and visualized using **Matplotlib and Seaborn**. A final dashboard was built in **Power BI**.

### **📆 Sales Trends**

* **November** recorded the highest revenue (~2.9M)
* **October** was the second-highest (~2.2M)
* Clear **Q4 spike** indicates holiday-driven demand
* Monthly fluctuations reveal seasonal buying behavior

### **📦 Product Performance**

Top products by revenue include:

* **REGENCY CAKESTAND**
* **DOTCOM POSTAGE**
* **WHITE HANGING HEART**
* **PARTY BUNTING**
* **JUMBO BAG RED**

These products consistently drive a major share of total revenue.

### **👥 Customer Analysis**

* Unique Customers: **~5,851**
* Top customers (IDs: **10, 18102, 14646**) contribute disproportionately high revenue
* Pareto pattern observed: **20% customers → 80% revenue**

### **🌎 Geographic Analysis**

Top revenue-generating countries:

* **United Kingdom**: 85%+ share
* Netherlands, Germany, France, Ireland contribute modest but promising revenue

### **↩️ Order Status / Returns**

* Negative quantities represent returns
* Returns are minimal but important for outlier handling and profitability insights

### **📏 Quantity & Pricing Patterns**

* Most purchases occur in **1–5 units**
* Quantity **100+ accounts for 15%+ of revenue**, indicating bulk buying
* UnitPrice mostly low, with some high-value outliers removed during cleaning

### **📅 Weekday Analysis**

* **Wednesday–Friday** → highest sales
* **Saturday** → lowest, showing weekend drop
* Useful for planning staffing & promotions

---

## 📊 **Dashboard Summary (Power BI)**

The Power BI dashboard includes:
<img width="1400" height="500" alt="monthly_revenue_trend (1)" src="https://github.com/user-attachments/assets/cf445928-2b31-4cee-93e3-4707c2380b27" />

<img width="1302" height="556" alt="download" src="https://github.com/user-attachments/assets/ed661811-1792-4c0e-959f-2ba1e5e45585" />
<img width="1152" height="787" alt="download (1)" src="https://github.com/user-attachments/assets/0da42d52-e137-453e-b402-6a0559e12c35" />


### **KPI Cards**

* **Total Revenue**
* **Average Sales**
* **Total Customers**
* **Total Invoices**

### **Visualizations**

* Top 10 Customers (bar chart)
* Top 10 Products (bar chart)
* Revenue by Country (map)
* QuantityBin distribution (donut chart)
* Monthly Revenue Trend (line chart)
* Yearly Revenue Summary (stacked bar chart)
* Weekday revenue (area / line chart)

### **Slicers**

* Month
* Country
* CustomerID
* QuantityBin

This enables dynamic exploration of sales performance.

---

## ⭐ **Key Insights**

* **Total Revenue:** ~**19.2M**
* **UK Dominance:** UK contributes **>85%** of revenue
* **High-Value Customers:** Top 5 customers drive significant revenue
* **Seasonal Trends:** Strong sales in **Oct–Nov**, indicating Q4 demand
* **Quantity Behavior:** Small quantities dominate, but bulk orders significantly boost revenue
* **Top Products:** A few products consistently outperform across the year
* **Weekday Pattern:** Wednesday–Friday strongest; Saturday weakest
* **Returns:** Minimal but valuable for data quality and profitability analysis

---

## 🏁 **Final Conclusion**

To improve business performance:

* Focus on **high-revenue products** with targeted advertising
* Strengthen bonds with **top customers** via loyalty incentives
* Prepare inventory for **Q4** seasonal demand
* Target **international expansion** outside the UK
* Develop separate strategies for **retail vs bulk buyers**
* Improve data logging for missing CustomerIDs and check pricing outliers

These actions will improve **revenue**, **customer retention**, and **inventory efficiency**.

---

## 🛠 **Methods Used**

### **Tools & Technologies**

* Python (Pandas, NumPy)
* Matplotlib & Seaborn
* Power BI

### **Techniques**

* Data Cleaning
* Feature Engineering
* Descriptive Statistics
* Time-Series Analysis
* Customer & Product Segmentation

### **Python Methods Used**

* `groupby()`, `value_counts()`, `agg()`
* `dt.month`, `dt.year`, `apply()`
* `describe()`, `corr()`

### **Visualization Types**

* Bar Charts
* Line Charts
* Donut Chart
* KPI Cards
* Heatmaps
* Pairplots
* Boxplots
* Histograms
* Country Map Chart

### **Analysis Focus**

* Revenue
* Customer segmentation
* Product performance
* Country-level sales
* Seasonal trends
* Outlier analysis

---





---

## 🛠️ How to Run the Project
1. Open `Online_Retail_EDA.ipynb` in **Google Colab**.  
2. Upload the dataset file (`online_retail_ii_UCI_data_set.csv`).  
3. Run all cells sequentially.  
4. Cleaned dataset will be saved as `online_retail_cleaned.csv`.  

---

## 👨‍💻 Author
**Purna Shekhar**  
Data Analyst | Python | Power BI | Excel | SQL  
📧 purnashekhar2352@gmail.com
🔗 www.linkedin.com/in/bandi-purnashekhar 
🔗 [GitHub](https://github.com/purnashekhar)

---

⭐ **If you found this project insightful, don’t forget to give it a star!** ⭐
