# 📊 Customer Churn Analysis — Telecom Dataset

## 📌 Project Overview
This project analyses customer churn behaviour for a telecom company using a dataset of 7,000+ records. The goal was to identify key drivers of churn and provide actionable insights that can help businesses improve customer retention strategies.

---

## 🎯 Business Problem
Customer churn is one of the most costly problems for subscription-based businesses. Acquiring a new customer costs 5–7x more than retaining an existing one. This analysis answers:
- Who is churning and why?
- Which customer segments are highest risk?
- What can the business do to reduce churn?

---

## 📁 Dataset
- **Source:** [Telco Customer Churn — Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Records:** 7,043 customers
- **Features:** 21 columns including contract type, tenure, monthly charges, internet service, and churn label

---

## 🛠️ Tools & Libraries
| Tool | Purpose |
|------|---------|
| Python | Core analysis |
| Pandas | Data cleaning & manipulation |
| Matplotlib | Data visualisation |
| Seaborn | Statistical visualisation |
| Google Colab | Development environment |

---

## 🔄 Project Workflow

### 1. Data Cleaning
- Converted `TotalCharges` from string to numeric
- Removed 11 null records
- Dropped `customerID` (non-analytical column)
- Encoded `Churn` column as binary (0/1)

### 2. Feature Engineering
- Created `Tenure Group` buckets: 0–12, 13–24, 25–48, 49–72 months for segmentation analysis

### 3. Exploratory Data Analysis (EDA)
Analysed churn across 6 dimensions:
- Overall churn distribution
- Churn by contract type
- Churn rate by tenure group
- Monthly charges vs churn
- Churn by internet service type
- Correlation heatmap of numeric features

### 4. Revenue Impact Analysis
- Calculated total monthly revenue lost to churned customers
- Quantified the exact % of revenue at risk to frame churn as a business problem, not just a metric

### 5. Annotated Insight Chart
- Added business context annotations directly onto the contract type chart
- Highlighted that month-to-month customers churn 14x more than two-year contract customers — communicating findings in a way non-technical stakeholders can act on

---

## 📈 Key Findings
- **Overall churn rate:** ~26%
- **Month-to-month contracts** had the highest churn rate at ~43% vs only ~3% for two-year contracts
- **New customers (0–12 months)** are the highest risk segment
- **Churned customers** paid ~$15 more per month on average than retained customers
- Customers without **tech support or online security** showed significantly higher churn
- **~$139,000+ in monthly revenue** is at risk from churned customers

---

## 💡 Business Recommendations
1. Offer discounts or loyalty incentives to month-to-month customers to convert them to longer contracts
2. Prioritise retention campaigns for customers in their first 12 months
3. Bundle tech support and online security into base plans to improve perceived value
4. Focus highest-effort retention on high monthly charge customers — they represent the biggest revenue risk

---

## 📂 Repository Structure
```
customer-churn-analysis/
│
├── churn_analysis.ipynb              # Main Colab notebook
├── WA_Fn-UseC_-Telco-Customer-Churn.csv  # Dataset (download from Kaggle)
├── charts/
│   ├── churn_distribution.png
│   ├── churn_by_contract.png
│   ├── churn_by_tenure.png
│   ├── monthly_charges_churn.png
│   ├── churn_by_internet.png
│   ├── correlation_heatmap.png
│   ├── revenue_impact.png
│   └── contract_churn_annotated.png
└── README.md
```
---

## 🚀 How to Run
1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
2. Open `churn_analysis.ipynb` in [Google Colab](https://colab.research.google.com/)
3. Upload the CSV file when prompted
4. Run all cells in order

---

## 👤 Author
**Aayush Tyagi**
[LinkedIn](https://www.linkedin.com/in/aayushtyagi003)
