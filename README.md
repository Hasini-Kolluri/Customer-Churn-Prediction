
# Telco Customer Churn Prediction

This project focuses on analyzing customer behavior and predicting churn using machine learning models. Churn prediction is crucial in the telecom industry to retain customers and reduce revenue loss.

## Problem Statement
> Predict whether a customer is likely to churn (i.e., leave the service) based on their demographic and service usage data.

## Dataset

 **Source:** Telco Customer Churn dataset (CSV)
 **Features include:**
   - Customer demographics (gender, senior citizen, tenure, etc.)
   - Services subscribed (internet, online security, streaming, etc.)
   - Billing info (monthly charges, total charges)
   - Target column: `Churn` (Yes/No)

## ML Workflow

### Data Preprocessing
 - Handled missing values using `SimpleImputer`
 - Applied encoding using `OneHotEncoder`
 - Scaled numerical features with `StandardScaler`
 - Built a preprocessing pipeline using `ColumnTransformer`

### Exploratory Data Analysis (EDA)
  Visualized categorical distributions.
  Explored churn patterns across services and tenure

### Models Trained
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Support Vector Machine (SVM)

### Hyperparameter Tuning
  - Performed `GridSearchCV` on each model
  - Compared models using accuracy, precision, recall, and F1-score

## Evaluation Metrics

| Metric     | Churn = Yes | Churn = No |
|------------|-------------|------------|
| Precision  | 0.71        | 0.86       |
| Recall     | 0.59        | 0.91       |
| F1-Score   | 0.64        | 0.89       |
| Accuracy   | 0.83        | -          |  

The model performs well overall, especially in identifying non-churning customers. However, there is room to improve recall for churn cases.
Potential improvements:
- Class balancing using SMOTE
- Using ensemble models like XGBoost or Gradient Boosting
- Applying SHAP for model explainability

## Author:
Hasini Kolluri  
2nd Year Undergraduate, Aspiring Machine Learning Engineer  
- GitHub: https://github.com/Hasini-Kolluri
- Project Repo: https://github.com/Hasini-Kolluri/Customer-Churn-Prediction

## Acknowledgements:
- Dataset from Kaggle
- Scikit-learn for modeling
