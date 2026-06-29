# Telco Customer Churn Analysis

End-to-end exploratory data analysis and machine learning project to identify key drivers of customer churn in the telecom industry.

---

## Project Overview

Customer churn is one of the most critical problems in the telecom industry. This project analyses a real-world telecom dataset to:
- Identify which customers are most likely to churn
- Understand the key factors driving churn
- Quantify revenue loss from churned customers
- Flag high-risk customers for targeted retention

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python | Core analysis language |
| Pandas | Data manipulation & cleaning |
| Matplotlib | Data visualisation |
| Seaborn | Statistical visualisation |
| Scikit-learn | KNN classification model |
| Google Colab | Development environment |

---

## Project Structure

```
Telco-Churn-Analysis/
│
├── Telco_Churn_Dataset_Analysis.ipynb   # Main analysis notebook
├── Telco_Customer_Churn.csv             # Dataset
└── README.md
```

---

## Key Findings

### Churn Distribution
- Dataset has a 73:27 churn imbalance — majority of customers did not churn
- Identified need for SMOTE to handle class imbalance in predictive modeling

### Tenure Analysis
- Tenure distribution is right-skewed — large number of customers leave very early
- First few months are critical for customer retention
- Moderate negative correlation of −0.35 between tenure and churn
- Customers with longer tenure are significantly less likely to churn

### Payment Method
- Electronic check users have the highest churn rate at 45%
- Payment method is strongly associated with churn behaviour

### Contract Type
- Month-to-month customers churn at a far higher rate
- 1-year and 2-year contract customers show significantly lower churn

### Monthly Charges
- Higher monthly charges are directly associated with higher churn
- Churned customers tend to be on higher-priced plans

### Revenue Impact
- Total revenue lost to churned customers: $139,130
- 1,237 high-risk customers identified (churned + above-median monthly charges)
- Revenue increases proportionally with customer tenure

---

## Model Building

- Applied one-hot encoding to categorical variables
- Split data into 80% train / 20% test
- Built a K-Nearest Neighbours (KNN) Classifier with k=5
- Evaluated using classification report and accuracy score

---

## Business Recommendations

1. Target early-tenure customers with onboarding support and loyalty offers
2. Incentivise long-term contracts to reduce month-to-month churn
3. Investigate electronic check friction — offer easier payment alternatives
4. Focus retention budget on the 1,237 identified high-risk customers
5. Use tenure as a key feature in future predictive churn models

---

## Connect

Sourav Prakash — Aspiring Data Analyst
- LinkedIn: linkedin.com/in/sourav-prakash-analyst
- GitHub: github.com/Sourav112004
- Email: souravprakash112004@gmail.com
