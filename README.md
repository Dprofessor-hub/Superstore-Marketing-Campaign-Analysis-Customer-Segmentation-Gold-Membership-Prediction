# 🤖 Superstore Marketing Campaign Analysis

### Customer Segmentation & Gold Membership Prediction

> **End-to-end Data Analytics Project** using Excel, Python, Statistics, Machine Learning, and Power BI.

---

## 📌 Project Overview

Superstore runs a year-end promotional campaign offering existing customers a **Gold Membership with a 20% discount on purchases**.

### 🎯 Objectives

- Identify customers most likely to accept the Gold Membership
- Understand customer demographics and purchasing behavior
- Identify high-value customer segments
- Analyze product-category and purchase-channel behavior
- Predict membership acceptance using Machine Learning
- Develop actionable marketing recommendations
- Optimize campaign targeting and marketing spend

### 📊 Dataset

| Metric | Value |
|---|---:|
| Customers | **2,213** |
| Features | **22** |
| Acceptance Rate | **15.04%** |
| Average Income | **₹52,247** |
| Average Total Spend | **₹606.78** |

---

## 🎯 Business Questions

1. What factors influence Gold Membership acceptance?
2. Which customer segments are most valuable and receptive?
3. Which product categories contribute most to customer spending?
4. Which purchase channels are strongest indicators of campaign response?
5. Can Machine Learning predict customers likely to accept the membership?
6. How can marketing budget be focused on high-probability customers?

---

## 🛠️ Tools & Technologies

| Category | Tools / Techniques |
|---|---|
| Data Validation | **Excel** |
| Data Cleaning | **Python, Pandas, NumPy** |
| Exploratory Data Analysis | **Python, Matplotlib** |
| Statistical Analysis | **T-Test, Chi-Square Test, ANOVA / Group Analysis** |
| Machine Learning | **Logistic Regression, Random Forest, SMOTE** |
| Data Visualization | **Power BI** |
| Documentation | **Report & Presentation** |

---

## 🔄 Project Workflow

```text
Raw Dataset
    ↓
Excel Data Validation
    ↓
Python Data Cleaning & Transformation
    ↓
Feature Engineering
    ↓
Exploratory Data Analysis
    ↓
Statistical Analysis
    ↓
Machine Learning
    ↓
Power BI Dashboard
    ↓
Business Insights & Recommendations
```

---

# 1️⃣ Excel — Data Validation

- Checked data integrity and field consistency
- Reviewed missing values and anomalies
- Validated demographic fields
- Validated spending and purchase-count fields
- Checked the campaign response field
- Prepared the dataset for further analysis

---

# 2️⃣ Python — Data Cleaning & EDA

Python was used for data preparation, transformation, feature engineering, and exploratory analysis.

### 🔧 Feature Engineering

- `Age`
- `Tenure`
- `Total_Spend`
- `Category_Breadth`
- Engagement / purchase-channel metrics
- Income bands
- Customer segments

### 📊 Exploratory Analysis

- Customer income
- Customer age
- Recency
- Product-category spending
- Purchase channels
- Education
- Marital status
- Household composition
- Campaign response

---

# 3️⃣ 📐 Statistical Analysis

Statistical tests were used to identify relationships between customer characteristics and membership acceptance.

| Analysis | Finding |
|---|---|
| **Education vs Response** | Chi-square test showed a significant association |
| **Marital Status vs Response** | Chi-square test showed a significant association |
| **Income vs Response** | Responders had significantly higher average income |

### 💡 Income Comparison

| Customer Group | Average Income |
|---|---:|
| Responders | **₹60,210** |
| Non-Responders | **₹50,824** |

---

# 4️⃣ 🤖 Machine Learning

The target variable was **`Response`**.

| Response | Meaning |
|---:|---|
| `1` | Customer accepted the Gold Membership |
| `0` | Customer did not accept |

### Models Implemented

- Logistic Regression
- Random Forest
- Random Forest + SMOTE

### ⚠️ Class Imbalance

- **1,880 Non-Responders**
- **333 Responders**

Responders represented only about **15%** of customers, so **SMOTE** was used to improve responder detection.

## 📊 Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 86% | 63% | 18% | 0.28 | 0.80 |
| Random Forest | 86% | 65% | 22% | 0.33 | 0.84 |
| **Random Forest + SMOTE** | **84%** | **47%** | **48%** | **0.47** | **0.83** |

### 🏆 Recommended Model — Random Forest + SMOTE

| Metric | Result |
|---|---:|
| Responders Correctly Identified | **32** |
| Original Random Forest | **15** |
| Recall | **22% → 48%** |
| F1 Score | **0.33 → 0.47** |

> In a marketing campaign, identifying more genuine prospects can be more valuable than maximizing overall accuracy.

### 🔎 Top Predictive Features

1. **Recency**
2. **Web/Store Ratio**
3. **Total Spend**
4. **Income**
5. **Tenure**
6. **Family Size**
7. **Store Purchases**

---

# 5️⃣ 📊 Power BI Dashboard

Two interactive dashboards were developed.

## Executive Summary Dashboard

### KPIs

- Membership Acceptance Rate
- Average Customer Income
- Average Total Spend

### Visualizations

- Membership Response Distribution
- Acceptance Rate by Education
- Average Spend by Product Category
- Acceptance Rate by Marital Status
- Executive Insights Panel

### Filters

- Marital Status
- Education

## Marketing Analytics Dashboard

### Visualizations

- Total Spend vs Recency by Response
- Acceptance Rate by Income Band
- Average Spend by Category: Responders vs Non-Responders
- Average Total Spend by Income Band

### Filters

- Family Size
- Response Label

---

# 6️⃣ 📈 Key Business Insights

## 💰 Campaign Performance

- **2,213 customers** were analyzed
- Overall Gold Membership acceptance rate was **15.04%**
- Average customer income was approximately **₹52,247**
- Average total spend over two years was **₹606.78**
- **Wine** was the highest-spending product category

## 👥 Customer Segmentation

- Higher-income customers were more likely to accept the membership
- Responders averaged **₹60,210** income vs **₹50,824** for non-responders
- **PhD and Master** customers showed stronger acceptance
- Smaller households showed higher acceptance than households with children/teenagers

## 🛒 Product Spending

Responders spent more than non-responders across **all six product categories**.

**Strongest spending differences:**

1. 🍷 Wine
2. 🥩 Meat Products
3. 🪙 Gold Products
4. 🐟 Fish Products
5. 🍬 Sweet Products
6. 🍎 Fruits

## 📱 Purchase Channels

| Channel | Key Insight |
|---|---|
| **In-Store** | Largest overall channel, but not a strong differentiator |
| **Web** | Responders had higher average web purchases |
| **Catalogue** | Strongest channel differentiator |
| **Deals / Discounts** | Very little difference between responders and non-responders |

### ⭐ Channel Comparison

| Channel | Responders | Non-Responders |
|---|---:|---:|
| Web Purchases | **5.07** | **3.91** |
| Catalogue Purchases | **4.20** | **2.40** |

---

# 7️⃣ 💡 Strategic Recommendations

### 1. 🎯 Target High-Income, High-Spend Customers

Prioritize customers with:

- Income above **₹55,000**
- Total spend above **₹400**

### 2. 📧 Prioritize Catalogue & Web Campaigns

Use catalogue and digital campaigns as primary targeting channels because they show stronger separation between responders and non-responders.

### 3. ⏱️ Time Offers Around Recent Purchases

**Recency was the strongest predictive feature.**

Target customers soon after their purchases while brand engagement is high.

### 4. 🔄 Re-Engage Dormant Customers

Customers with high recency and low spending should receive a **re-engagement campaign first** before being targeted for membership.

### 5. 👨‍👩‍👧 Adapt Offers for Family Households

Customers with children or teenagers showed lower acceptance. Consider **family-oriented membership benefits**.

### 6. 🤖 Use ML Scores for Campaign Prioritization

Use the **Random Forest + SMOTE** model to score customers and prioritize personalized outreach toward the highest-probability customers.

---

# 8️⃣ 📂 Repository Structure

```text
Superstore-Marketing-Campaign-Analysis/
│
├── data/
│   ├── Superstore Marketing Campaign Dataset.csv
│   └── Superstore_cleaned.csv
│
├── dashboard/
│   └── SuperStore Dashboard.pbix
│
├── reports/
│   └── REPORT ON SUPERSTORE MARKETING CAMPAIGN FOR GOLD CARD.pdf
│
├── presentation/
│   └── Super Store Presentation.odp
│
├── problem-statement/
│   └── Capstone Problem Statement - Superstore Marketing Campaign Analysis.pdf
│
├── images/
│   ├── executive-dashboard.png
│   └── marketing-dashboard.png
│
└── README.md
```

---

# 9️⃣ 🖥️ Dashboard Preview

## Executive Summary

<img width="1655" height="917" alt="Screenshot 2026-08-11 131358" src="https://github.com/user-attachments/assets/9f18edbf-df0f-4e5e-8664-ad72bf1e2556" />


## Marketing Analytics

<img width="1655" height="925" alt="Screenshot 2026-08-11 131417" src="https://github.com/user-attachments/assets/42fcc9dc-25c7-4910-b823-7f75b041ac6e" />

---

# 🔟 🎯 Final Outcome

This project demonstrates a complete **end-to-end Data Analytics workflow**:

```text
Data → Cleaning → EDA → Statistics → Machine Learning → Dashboard → Insights → Recommendations
```

### Skills Demonstrated

- Excel Data Analysis
- Python & Pandas
- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis
- Statistical Testing
- Machine Learning
- SMOTE & Class Imbalance Handling
- Power BI Dashboard Development
- Customer Segmentation
- Business Analysis
- Data-Driven Recommendations

### Business Value

The analysis helps the marketing team:

- Identify high-value customers
- Improve campaign targeting
- Prioritize effective marketing channels
- Identify likely membership responders
- Reduce inefficient marketing spend
- Make data-driven campaign decisions

---

# 👨‍💻 Author

### Dipanshu Rangari

**Data Analyst**

**Skills:** Excel | SQL | Python | Power BI | Tableau | Statistics | Machine Learning

🔗 **GitHub:**  
https://github.com/Dprofessor-hub

---

# ⭐ Key Takeaway

> **The strongest membership prospects are recent, high-income, high-spending customers who are actively engaged through web and catalogue channels — making targeted outreach more effective than a broad campaign.**

---

## 📚 Project Documentation

This repository also contains:

- Problem Statement
- Original Dataset
- Cleaned / Engineered Dataset
- Power BI Dashboard
- Project Report
- Project Presentation
