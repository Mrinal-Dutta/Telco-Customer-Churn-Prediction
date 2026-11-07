# Telco Customer Churn Prediction

## Project Overview
This project focuses on predicting customer churn for a telecommunications company using Machine Learning.

The objective is to identify customers who are likely to leave the company and help businesses develop effective customer retention strategies.

## Business Problem
Customer churn directly impacts business revenue. Identifying customers who are likely to leave can help companies take proactive retention measures.

## Dataset
- Dataset: IBM Telco Customer Churn
- Total Records: 7,043
- Total Original Features: 21
- Target Variable: Churn

## Project Workflow
1. Data Collection
2. Data Cleaning and Preprocessing
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Model Building
6. Model Evaluation
7. Threshold Tuning
8. Final Model Selection

## Machine Learning Models
- Logistic Regression
- Balanced Logistic Regression
- Decision Tree
- Random Forest

## Model Performance

Final Selected Model: Balanced Logistic Regression

| Metric | Test Score |
|---|---:|
| Accuracy | 77.36% |
| Precision | 56% |
| Recall | 71% |
| F1-Score | 63% |
| ROC-AUC | 0.842 |

Selected Classification Threshold: 0.6

## Key Business Insights
- Month-to-month contract customers show higher churn.
- Customers with shorter tenure are more likely to leave.
- Electronic check users have relatively higher churn.
- Fiber optic customers show relatively higher churn.
- Customers without online security and tech support show higher churn.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure
```text
Telco-Customer-Churn-Prediction/
│
├── data/
│   ├── WA_Fn-UseC_-Telco-Customer-Churn.csv
│   └── processed/
│       └── cleaned_customer_churn.csv
│
├── models/
│   └── customer_churn_model.pkl
│
├── notebook/
│   ├── 01_Data_Collection_and_Cleaning.ipynb
│   └── 02_Exploratory_Data_Analysis.ipynb
│
└── README.md
```

## Conclusion
This project demonstrates how Machine Learning can be used to predict customer churn and support data-driven customer retention strategies.

The final model achieved a ROC-AUC score of 0.842 on the test dataset.
## Model Performance Comparison

Four classification models were evaluated using the test dataset.

| Model | Accuracy | Churn Recall | ROC-AUC |
|---|---:|---:|---:|
| Logistic Regression | 0.7991 | 0.5187 | 0.8424 |
| Balanced Logistic Regression | 0.7324 | 0.7914 | 0.8422 |
| Decision Tree | 0.7282 | 0.4813 | 0.6498 |
| Random Forest | 0.7651 | 0.6310 | 0.8244 |

## Final Model Selection

Balanced Logistic Regression was selected as the preferred model because it achieved the highest churn recall of 79.14%.

- Correctly identified 296 out of 374 actual churn customers.
- Achieved a ROC-AUC score of 0.8422.
- Helps identify more potential churn customers.

The model has lower accuracy than standard Logistic Regression and produces more false positives. The final choice should consider the business cost of these errors.

## Key Business Insights

- Month-to-month contract customers show a higher churn rate.
- Customers with shorter tenure are more likely to churn.
- Electronic check users have a higher churn rate.
- Fiber optic customers show relatively higher churn.
- Customers without online security and tech support show higher churn.

## Business Recommendations

- Encourage customers to choose long-term contracts.
- Offer special retention plans to new customers.
- Improve fiber optic service quality.
- Promote automatic payment methods.
- Encourage customers to use online security and technical support services.
