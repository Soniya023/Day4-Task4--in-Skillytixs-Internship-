# Day4-Task4--in-Skillytixs-Internship-
Predicting customer churn in telecom using machine learning.

## Project Overview

Customer churn is a critical metric in the telecom industry, representing customers who leave the service.  
This project uses machine learning to predict whether a customer will churn based on their demographic, account, and usage data.  
By identifying potential churners early, telecom companies can take preventive actions to improve customer retention.

## Tools & Libraries

- Python  
- Pandas, NumPy – Data manipulation  
- Matplotlib, Seaborn – Data visualization  
- Scikit-Learn – Machine Learning models and preprocessing  
- Joblib – Save and load trained models  

## Dataset

- Source: [Kaggle – Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)  
- Features include:  
  - Customer demographics (gender, senior citizen, partner, dependents)  
  - Account information (tenure, contract type, payment method, monthly charges)  
  - Service usage (internet, phone, streaming, backup, support)  
  - Target variable: **Churn** (Yes/No)

## Project Workflow

1. Data Cleaning & Preprocessing  
   - Handle missing values (e.g., `TotalCharges`)  
   - Encode categorical variables (LabelEncoder for binary, OneHotEncoder for multi-class)  
   - Scale numeric features  

2. Train-Test Split  
   - Split dataset into training and testing sets (80-20 split)  

3. Model Training  
   - Random Forest Classifier  
   - Optional: Logistic Regression for comparison  

4. Evaluation  
   - Accuracy, classification report, confusion matrix, ROC-AUC  
   - Feature importance visualization  

5. New Customer Prediction  
   - Predict churn probability for new customer data  

6. Model Saving  
   - Save model and scaler using Joblib for future deployment

## Key Results & Insights

- Top features affecting churn: `tenure`, `MonthlyCharges`, `Contract type`, `Payment method`, `Internet service type`  
- Random Forest achieved high accuracy and ROC-AUC scores  
- Customers with short tenure and high monthly charges are more likely to churn  

## How to Use

1. Clone the repository:  
   ```bash
   git clone https://github.com/username/Telco-Customer-Churn.git
