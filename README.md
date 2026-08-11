# 🤖 Superstore Marketing Campaign Analysis

Customer Segmentation & Gold Membership Prediction

End-to-end Data Analytics Project using Excel, Python, Statistics, Machine Learning and Power BI.

# 📌 Project Overview

Superstore runs a year-end promotional campaign offering existing customers a Gold Membership with a 20% discount on purchases.

The objective is to understand:

Which customers are most likely to accept the offer

Which customer segments are most valuable and receptive

How purchasing behavior differs across customers

Which channels are strongest indicators of campaign response

How marketing budget can be focused on high-probability customers

Dataset: 2,213 customers | 22 features

The dataset covers:

Demographics

Household composition

Income

Recency

Product-category spending

Purchase channels

Complaints

Campaign response

# 🎯 Business Questions

#

Business Question

1

What factors influence Gold Membership acceptance?

2

Which customer segments are most valuable and receptive?

3

Which product categories contribute most to customer spend?

4

Which purchase channels are strongest indicators of campaign response?

5

Can machine learning predict customers likely to accept the membership?

6

How can marketing budget be focused on high-probability customers?

# 🛠️ Tools & Technologies

Area

Tools / Techniques

Data Validation & Initial Analysis

Excel

Data Cleaning & Transformation

Python, Pandas, NumPy

Exploratory Data Analysis

Python, Matplotlib

Statistical Analysis

T-test, Chi-square Test, ANOVA / group analysis

Machine Learning

Logistic Regression, Random Forest, SMOTE

Business Intelligence

Microsoft Power BI

Documentation

Report & Presentation

# 📊 Project Workflow

Raw Dataset
     ↓
Excel Validation
     ↓
Python Cleaning & Feature Engineering
     ↓
Exploratory Data Analysis
     ↓
Statistical Analysis
     ↓
Machine Learning Modeling
     ↓
Power BI Dashboard
     ↓
Business Insights & Recommendations

1️⃣ Excel — Data Validation

Checked data integrity and field consistency.

Reviewed missing values and anomalies.

Validated demographic, spending, purchase-count, and response fields.

Prepared the dataset for further analysis.

2️⃣ Python — Data Preparation & EDA

Performed data cleaning, transformation, feature engineering, and exploratory analysis.

Key engineered metrics:

Age

Tenure

Total_Spend

Category_Breadth

Engagement / purchase-channel metrics

Income bands and customer segments

EDA focused on:

Income

Recency

Spending behavior

Product categories

Demographics

Household composition

Purchasing channels

3️⃣ Statistical Analysis

Statistical testing was used to determine whether important customer characteristics were associated with campaign acceptance.

Examples:

Education vs Response: Chi-square test showed a significant association.

Marital Status vs Response: Chi-square test showed a significant association.

Income: Responders had significantly higher average income than non-responders.

4️⃣ Machine Learning

The target variable was Response:

Response

Meaning

1

Customer accepted the Gold Membership

0

Customer did not accept

Models evaluated:

Logistic Regression

Random Forest

Random Forest + SMOTE

Because responders represented only about 15% of customers, SMOTE was used to address class imbalance.

5️⃣ Power BI Dashboard

Two interactive dashboard views were developed.

Executive Summary Dashboard

Membership Acceptance Rate

Average Customer Income

Average Total Spend

Response distribution

Acceptance by Education

Acceptance by Marital Status

Average Spend by Product Category

Executive insights panel

Demographic filters

Marketing Analytics Dashboard

Total Spend vs Recency by Response

Acceptance Rate by Income Band

Average Spend by Category: Responders vs Non-Responders

Average Total Spend by Income Band

Family Size filter

Response Label filter

📈 Key Business Insights

Campaign Performance

KPI

Value

Customers Analyzed

2,213

Gold Membership Acceptance Rate

15.04%

Average Customer Income

₹52,247

Average Total Spend — 2 Years

₹606.78

Highest-Spending Product Category

Wine

Customer Segmentation

Higher-income customers were more likely to accept the membership.

Responders had an average income of ₹60,210, compared with ₹50,824 for non-responders.

Higher education groups, particularly PhD and Master customers, showed stronger acceptance.

Customers with smaller households showed higher acceptance than households with children/teenagers.

Product Spending

Responders spent more than non-responders across all six product categories.

Strongest spending differences:

🍷 Wine

🥩 Meat Products

🪙 Gold Products

🐟 Fish Products

🍬 Sweet Products

🍎 Fruits

Purchase Channels

Channel

Key Finding

In-Store

Largest overall purchase channel, but not a strong differentiator

Web

Responders averaged more web purchases than non-responders

Catalogue

Strongest channel differentiator

Deals / Discounts

Very little difference between responders and non-responders

# 🤖 Machine Learning Results

The dataset had significant class imbalance:

1,880 non-responders vs 333 responders

Model Comparison

Model

Accuracy

Precision

Recall

F1

ROC-AUC

Logistic Regression

86%

63%

18%

0.28

0.80

Random Forest

86%

65%

22%

0.33

0.84

Random Forest + SMOTE

84%

47%

48%

0.47

0.83

# 🏆 Selected Model — Random Forest + SMOTE

Although accuracy decreased slightly, the SMOTE model improved the ability to identify actual responders.

Metric

Result

Responders correctly identified

32

Original Random Forest

15

Recall

22% → 48%

F1 Score

0.33 → 0.47

For a marketing campaign, identifying more genuine prospects is more valuable than maximizing overall accuracy alone.

🔎 Top Predictive Features

Recency

Web/Store Ratio

Total Spend

Income

Tenure

Family Size

Store Purchases

# 💡 Strategic Recommendations

1️⃣ Target High-Income, High-Spend Customers

Prioritize customers with:

Income above ₹55,000

Total spend above ₹400

2️⃣ Prioritize Catalogue & Web Campaigns

Use catalogue and digital campaigns as primary targeting channels because they show stronger separation between responders and non-responders.

3️⃣ Time Offers Around Recent Purchases

Recency was the strongest predictive feature.

Customers who purchased recently should receive membership offers while engagement is high.

4️⃣ Re-engage Dormant Customers First

Customers with high recency and low spending should receive a re-engagement campaign before being targeted for membership.

5️⃣ Adapt the Offer for Family Households

Customers with children or teenagers showed lower acceptance.

Consider family-oriented benefits rather than using a one-size-fits-all membership offer.

6️⃣ Use ML Scores for Campaign Prioritization

Use the Random Forest + SMOTE model to score customers and focus personalized outreach on the highest-probability segment instead of contacting everyone equally.

# 📂 Suggested Repository Structure

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

Rename the uploaded files/folders as needed when organizing the GitHub repository. Avoid committing confidential or sensitive business data if the dataset is not publicly shareable.

# 🖥️ Dashboard Preview

Executive Summary



Marketing Analytics



# 🎯 Final Outcome

This project demonstrates an end-to-end analytical workflow—from raw customer data to business recommendations.

The analysis combines:

Descriptive analytics

Statistical testing

Predictive modeling

Interactive Power BI reporting

The goal is to help a marketing team:

Identify high-value customers

Improve campaign targeting

Use marketing resources more efficiently

# 👨‍💻 Author

Dipanshu Rangari

Data Analyst | Excel | SQL | Python | Power BI | Tableau | Statistics | Machine Learning

🔗 GitHub: Dprofessor-hub

# ⭐ Key Takeaway

The strongest membership prospects are recent, high-income, high-spending customers who are actively engaged through web and catalogue channels—making targeted outreach more effective than a broad campaign.
