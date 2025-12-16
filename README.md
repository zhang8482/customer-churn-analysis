# Customer Churn Analysis (Python)

## Project Overview
This project analyzes customer churn behavior using an e-commerce dataset.
The objective is to identify key factors associated with customer churn and
build predictive models to support customer retention strategies.

## Dataset
- Approximately 5,600 customer records
- Target variable: `Churn` (0 = Retained, 1 = Churned)
- Features include customer demographics, usage behavior, satisfaction level,
  complaints, and transactional attributes

> Note: The original dataset is not publicly shared.  
> This repository focuses on the analysis workflow and modeling approach.

## Data Cleaning & Preprocessing
- Replaced invalid blank values with missing values
- Filled missing numerical values using median imputation
- Encoded categorical variables:
  - Binary features using Label Encoding
  - Multi-category features using One-Hot Encoding
- Standardized numerical features using `StandardScaler`

## Exploratory Data Analysis
Key insights from the analysis:
- Overall churn rate is approximately **16.8%**
- New customers (0–3 months tenure) have the highest churn risk
- Customers who submitted complaints show churn rates above **30%**
- Longer customer tenure is strongly associated with lower churn probability

## Modeling
Two machine learning models were trained and evaluated:
- Logistic Regression
- Decision Tree Classifier

### Model Performance (Test Set)
| Model | Accuracy | Precision | Recall | F1-score |
|------|---------|-----------|--------|---------|
| Logistic Regression | ~0.88 | ~0.71 | ~0.45 | ~0.55 |
| Decision Tree | ~0.92 | ~0.75 | ~0.76 | ~0.75 |

## Tools & Libraries
- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn

## Conclusion
Customer churn is strongly influenced by tenure and customer complaints.
Early-stage customers and dissatisfied users represent the highest churn risk.
Targeted onboarding strategies and effective complaint resolution could
significantly improve customer retention.
