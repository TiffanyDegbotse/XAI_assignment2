# XAI_assignment2
# Telco Customer Churn Prediction & Explainable AI 

## Project Description  
This project aims to analyze and predict customer churn for a telecommunications company using the Telco Customer Churn dataset. The goal is not only to build predictive models (Linear Regression, Logistic Regression, GAM) but also to ensure interpretability through assumption checks and explainable AI techniques.

## Dataset  
- **Dataset:** `WA_Fn-UseC_-Telco-Customer-Churn.csv` from Kaggle  
- **Size:** ~7,000 customers, 20+ features (numeric and categorical)  
- **Target:** `Churn` (Yes / No)  
- **Key Features:** Tenure, MonthlyCharges, TotalCharges, Contract type, Service features, Payment method, etc.

## Objectives  
1. Explore data and check modeling assumptions (linearity, independence, multicollinearity, etc.)  
2. Build and compare models: Linear Regression (as baseline), Logistic Regression, and Generalized Additive Model (GAM)  
3. Evaluate models using appropriate metrics (Accuracy, AUC, Precision, Recall, F1, R² for linear baseline)  
4. Use explainability tools (partial dependence, VIF, Cook’s distance, residuals, etc.) to interpret model behavior.

## Methods  
- **Preprocessing:** Handling missing values (TotalCharges), encoding categorical variables, scaling numeric features  
- **Models built:**  
  - Linear Regression (treating churn as continuous)  
  - Logistic Regression  
  - Logistic GAM  

## Evaluation Metrics  
- Accuracy, AUC for classification  
- Precision / Recall / F1 per class  
- R² and MSE for linear regression baseline  
- Confusion matrix, ROC curve  

## Key Results  
- Logistic Regression & GAM outperform Linear Regression by a significant margin  
- GAM captures non-linear relationships (e.g. for tenure, charges)  
- Best performance in terms of AUC ~0.86; accuracy ~0.81–0.82
- Logistic Regression had similar performance
- Both models struggle more with detecting churners (lower recall for churn class)  

## Interpretability Insights  
- Important features: Tenure, MonthlyCharges, TotalCharges, Contract type, InternetService  
- Effects: Short tenure & high charges increase churn risk; non-linear trends in total charges  
- Multicollinearity detected especially among billing-related numeric features and dummy encoded services  

## How to Run  
1. Clone the repo  
2. Run the notebook
