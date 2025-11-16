<!-- PROJECT BANNER -->
<p align="center">
  <img src="https://i.ibb.co/vjsqBqC/marketing-banner-blue.png" alt="Project Banner" width="100%">
</p>

<h1 align="center">📊 Marketing Campaign Analysis</h1>
<p align="center">Data Cleaning • EDA • Feature Engineering • Machine Learning</p>

<p align="center">
  <!-- Google Colab Badge -->
  <a href="https://colab.research.google.com/drive/1Mgtdae5iZdQDUBJ_tRiPyTXPHn9aPZIy">
    <img src="https://colab.research.google.com/assets/colab-badge.svg">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue">
  <img src="https://img.shields.io/badge/Pandas-Data%20Processing-green">
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-orange">
  <img src="https://img.shields.io/badge/Numpy-Arrays-red">
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-blue">
  <img src="https://img.shields.io/badge/Seaborn-Statistics-purple">
  <img src="https://img.shields.io/badge/Google-Colab-yellow">
  <img src="https://img.shields.io/badge/Status-Completed-success">
</p>

---

# 📑 Table of Contents
- [Project Overview](#project-overview)
- [Repository Structure](#repository-structure)
- [Dataset Summary](#dataset-summary)
- [Task 1 — Data Cleaning](#task-1--data-cleaning)
- [Task 2 — Exploratory Data Analysis](#task-2--exploratory-data-analysis)
- [Task 3 — Machine Learning Modeling](#task-3--machine-learning-modeling)
- [Feature Importance](#feature-importance)
- [Business Insights](#business-insights)
- [How to Run](#how-to-run)
- [Future Improvements](#future-improvements)
- [Author](#author)

---

# 📌 Project Overview
This project analyzes a marketing campaign dataset to uncover customer behavior patterns and predict whether a customer will **respond** to a promotional offer.

The project includes:

✔ Data Cleaning  
✔ Exploratory Data Analysis (EDA)  
✔ Feature Engineering  
✔ Outlier Detection  
✔ Machine Learning Models  
✔ Business insights  

This serves as a complete **end-to-end data analytics & machine learning workflow**.

---

# 📁 Repository Structure
```
marketing-campaign-analysis/
│
├── cleaned_marketing_campaign.csv
├── marketing_project_files.zip
├── changes_summary.txt
├── requirements.txt
└── README.md
```

---

# 🗂️ Dataset Summary
The dataset contains:

- 👤 **Customer demographics:** age, income, education  
- 🏠 **Household info:** kids, teens at home  
- 🛍️ **Purchasing behavior:** wines, meat, fruits, fish, sweets  
- 💻 **Engagement:** website, catalog & store purchases  
- ⏳ **Recency:** days since last purchase  
- 🎯 **Target variable:** response (0 = no, 1 = yes)  

---

# 🧼 Task 1 — Data Cleaning

### ✔ Cleaning Tasks Done
- Removed duplicate records  
- Imputed missing numeric values using **median**  
- Filled missing categorical values using **mode**  
- Cleaned string fields (trimmed, lowercase)  
- Converted date columns into proper datetime format  
- Renamed all columns into **snake_case** format  

### ✔ Engineered Features
- **age = 2025 - year_birth**  
- **total_spent** = sum of all product spending columns  
- **total_children = kidhome + teenhome**  

---

# 📊 Task 2 — Exploratory Data Analysis

### 🔹 Univariate Analysis
- Income distribution  
- Age distribution  
- Product spending distribution  
- Response rate  

### 🔹 Bivariate Analysis
- Income vs Total Spending  
- Recency vs Response  
- Scatterplots, barplots, pairplots  

### 🔹 Multivariate Analysis
- Correlation heatmap  
- Checking multicollinearity  
- Outlier detection  

### 🌟 Key Insights from EDA
- High-spending customers respond more often  
- Digitally engaged customers (web purchases) show higher response rates  
- Customers with recent activity have significantly higher conversion  
- Income positively influences both spending and response  

---

# 🤖 Task 3 — Machine Learning Modeling

### 🎯 Objective  
Predict if a customer will respond to a marketing campaign.

### ✔ Features Used
```
age, income, total_spent, total_children,
recency, numwebpurchases, numcatalogpurchases, numstorepurchases
```

### ✔ Preprocessing Steps
- Median imputation  
- StandardScaler for feature scaling  
- Train-test split (80/20, stratified)  

---

# 🔹 Model 1: Logistic Regression

### 📈 Performance Metrics

| Metric | Score |
|--------|--------|
| **Accuracy** | 0.8616 |
| **Precision** | 0.6087 |
| **Recall** | 0.2089 |
| **F1 Score** | 0.3111 |

### 📌 Interpretation
- High accuracy due to class imbalance  
- Low recall → many responders not detected  
- Good baseline model but not suitable for marketing targeting  

---

# 🔹 Model 2: Random Forest Classifier

### 📈 Performance Metrics

| Metric | Score |
|--------|--------|
| **Accuracy** | 0.8795 |
| **Precision** | 0.7407 |
| **Recall** | 0.2985 |
| **F1 Score** | 0.4255 |

### 📌 Interpretation
- Stronger performance in every metric  
- Higher precision & recall → detects more responders  
- Recommended model for real-world deployment  

---

# ⭐ Feature Importance
Ranked feature importance:

1. **total_spent**  
2. **numwebpurchases**  
3. **income**  
4. **recency**  
5. **numcatalogpurchases**  

These features drive marketing response behavior.

---

# 💼 Business Insights

### 💡 Key Findings
- Higher spenders respond more to campaigns  
- Digital customers are more engaged  
- Recent activity strongly correlates with acceptance  
- Income influences purchasing power and response  

### 🎯 Recommendations
- Focus marketing on **high-spending segments**  
- Prioritize **digital marketing channels**  
- Launch campaigns targeting **recently active customers**  
- Segment customers using spending + engagement metrics  

---

# 🛠️ How to Run

### Install dependencies:
```
pip install -r requirements.txt
```

### Open the notebook:
- Google Colab  
- Jupyter Notebook  
- VS Code  

Click the Colab badge at the top for direct execution.

---

# 🔮 Future Improvements
- Hyperparameter tuning using GridSearchCV  
- Handle class imbalance via SMOTE  
- Add boosting models (XGBoost, LightGBM)  
- Deploy using FastAPI  
- Build a Streamlit dashboard for visualization  

---

# 👨‍💻 Author

**Bishal Kumar Mishra**  
Data Analyst | Machine Learning Enthusiast  

📌 GitHub:   
📌 LinkedIn: https://www.linkedin.com/in/bishal-kumar-mishra-5359a9362/

---

<p align="center">⭐ If you found this project helpful, please consider giving it a star!</p>
