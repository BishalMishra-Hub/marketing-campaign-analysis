# 📊 Marketing Campaign Analysis — Data Cleaning, EDA & Machine Learning

A complete end-to-end data analytics project analyzing a marketing campaign dataset.  
This project includes **data cleaning**, **exploratory data analysis**, **feature engineering**, and **machine learning** to predict customer response and extract business insights.

---

## 🚀 Project Highlights
- Cleaned and standardized raw marketing data
- Performed detailed EDA (univariate, bivariate, multivariate)
- Built ML models: **Logistic Regression** and **Random Forest**
- Identified top behavioral drivers of customer response
- Delivered business insights for marketing strategy

---

## 📁 Repository Structure
```
marketing-campaign-analysis/
│
├── data/
│   └── cleaned_marketing_campaign.csv
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_EDA.ipynb
│   └── 03_modeling.ipynb
│
├── reports/
│   └── plots/
│
├── changes_summary.txt
├── requirements.txt
└── README.md
```

---

## 📌 Dataset Description
The dataset contains customer purchase behavior, demographics, and campaign response information.

Key columns include:
- `year_birth`, `education`, `marital_status`, `income`
- `kidhome`, `teenhome`
- `recency`, `numwebpurchases`, `numcatalogpurchases`
- Spending columns: `mntwines`, `mntmeatproducts`, etc.
- Target: **response** (0 = No, 1 = Yes)

---

# 🧹 Task 1 — Data Cleaning & Preprocessing

### ✔ Steps Completed
- Removed duplicate records  
- Filled missing numeric values (median)  
- Filled missing categorical values (mode)  
- Cleaned/standardized text fields  
- Converted date columns to datetime  
- Consistent snake_case column names  

### ✔ Feature Engineering
- `age = 2025 - year_birth`
- `total_spent = sum of all spending`
- `total_children = kidhome + teenhome`

📁 Output file: **cleaned_marketing_campaign.csv**

---

# 📊 Task 2 — Exploratory Data Analysis (EDA)

### ✔ Univariate Analysis
- Age distribution  
- Income histogram  
- Product spending distribution  
- Response rate visualization  

### ✔ Bivariate Analysis
- Income vs Spending  
- Recency vs Response  
- Spending patterns vs Response  

### ✔ Multivariate Analysis
- Correlation heatmap  
- Outlier detection via boxplots  

### 🔍 Key EDA Insights
- Majority customers are **30–60 years** old  
- Higher spending → higher response probability  
- Recency strongly influences response  
- Web buyers respond more than catalog/store buyers  

---

# 🤖 Task 3 — Machine Learning Modeling

### ✔ Features Used
`age`, `income`, `total_spent`, `total_children`,  
`recency`, `numwebpurchases`, `numcatalogpurchases`, `numstorepurchases`

### ✔ Data Preparation
- Median imputation  
- Train-test split (80/20, stratified)  
- Standard scaling for Logistic Regression  

---

## 🔹 Model 1: Logistic Regression
- Used as baseline model  
- Provides interpretable coefficients  

**Metrics:**  
Replace with your results:
- Accuracy: XX%  
- Precision/Recall/F1: from your output  

---

## 🔹 Model 2: Random Forest Classifier
- Handles non-linear relationships  
- Better performance on imbalanced data  
- Provides feature importance  

**Metrics:**  
Replace with your results:
- Accuracy: XX%  
- Classification report values  

### ⭐ Top Predictive Features
1. total_spent  
2. numwebpurchases  
3. income  
4. recency  
5. numcatalogpurchases  

---

# 📈 Business Insights

### 💡 Key Findings
- High spenders respond significantly more  
- Digital buyers (web purchases) respond best  
- Recently active customers are most valuable  
- Income positively impacts response  

### 🎯 Recommendations
- Target high-spending customer segments  
- Strengthen digital marketing channels  
- Offer personalized campaigns for recent customers  

---

# 🛠️ How to Run This Project

### Install dependencies:
```
pip install -r requirements.t
