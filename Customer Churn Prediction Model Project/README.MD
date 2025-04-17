# Customer Churn Prediction – Logistic Regression 

## Project Overview

This project analyzes customer churn using the Telco Customer Churn dataset. It aims to predict whether a customer is likely to cancel their subscription based on demographic, service usage, and billing features. The project demonstrates the full data science workflow, including data preprocessing, exploratory analysis, feature engineering, model training, and evaluation.

---

## Objective

To build a classification model that can accurately identify churned customers and provide actionable insights for customer retention strategies.

---

## Tools & Libraries

- Python
- pandas, numpy
- seaborn, matplotlib
- scikit-learn

---

## Dataset

**Source**: Telco Customer Churn (public dataset)

**Features include:**
- Demographic information: Gender, Senior Citizen, Dependents
- Subscription details: Contract type, Internet Service, Tech Support
- Billing data: Monthly Charges, Total Charges
- Target variable: Churn (Yes/No)

---

## Workflow Summary

1. **Data Cleaning**
   - Removed irrelevant fields (e.g., geographic info, customer IDs)
   - Converted Total Charges to numeric
   - Dropped missing entries

2. **Exploratory Data Analysis (EDA)**
   - Analyzed churn rates across contract types, support services, and payment methods
   - Found that shorter contracts and lack of tech support strongly correlated with higher churn

3. **Feature Encoding & Scaling**
   - Applied label encoding to categorical features
   - Scaled numeric features using StandardScaler

4. **Modeling**
   - Used Logistic Regression as a baseline model
   - Achieved balanced performance with high recall for churned customers

---

## Model Evaluation

**Model Used**: Logistic Regression (with scaled features)  
**Train/Test Split**: 80/20

**Accuracy**: 90.4%  
**Recall for Churned Customers**: 83%  
**Precision for Churned Customers**: 81%

**Confusion Matrix**:
             Predicted
              No    Yes
Actual  No    [962, 73]
        Yes   [67, 307]

## Key Insights

- Customers on month-to-month contracts are significantly more likely to churn
- Lack of tech support and online security is associated with higher churn rates
- Total tenure is a strong predictor of retention – longer-tenured customers tend to stay

---

## Future Improvements

- Implement Random Forest and Gradient Boosting classifiers for comparison
- Perform hyperparameter tuning with cross-validation
- Include ROC-AUC and SHAP explanations for model transparency

---

## Author

**Muhammadh Asbar**  
Master of IT (Enterprise Management), University of South Australia  
LinkedIn: [www.linkedin.com/in/muhammadh-asbar]  
