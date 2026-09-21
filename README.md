# Telecom Customer Churn Analysis

## Business Problem
Which customers are about to leave — and what should the retention team do about it first?

## Notebooks
- `1_eda_and_preprocessing.ipynb` — Exploratory analysis using a Power BI churn-risk dashboard, converting categorical variables to numeric, initial pattern identification (service calls, monthly charges, contract type)
- `2_hypothesis_testing_and_modeling.ipynb` — Welch's t-test (service calls), two-tailed t-test (monthly charges), and a logistic regression model to combine predictors into a churn probability score

## Dataset
Telecom customer records including contract type, monthly charges, service call 
history, and churn status. 

## Methodology
1. Explored churn patterns via a Power BI dashboard to identify candidate drivers
2. Formally tested two of those patterns using Welch's t-test and a two-tailed t-test
3. Built a logistic regression model combining multiple predictors to generate a 
   single churn-probability score per customer

## How to Run
Open either notebook in Google Colab or Jupyter. Requires: pandas, scikit-learn, 
statsmodels, matplotlib.

## Key Findings
- Logistic regression model reached 88% accuracy, correctly flagging 71% of churners before departure
- Contract type was the strongest predictor: 46% churn on month-to-month vs. 3% on two-year contracts
- Customers with 3+ service calls churned at a 94% rate (Welch's t-test, p < 0.001)
- Churned customers paid $7.89/month more on average (p < 0.001), linked to competitor-driven churn rather than pure price sensitivity

## Tools
Python (pandas, scikit-learn, statsmodels), Power BI

## Full Case Study
[Read the full write-up on my portfolio →](your-framer-link.com/projects/telecom-churn)
