# Telco-Customer-Churn-Analysis - End-to-End Data Science Project

This project is an end-to-end customer churn analysis and prediction case study using the Telco Customer Churn dataset. The goal is to understand churn behaviour, identify key churn drivers, build machine learning models to predict churn, and generate actionable business recommendations to improve customer retention.

This project demonstrates practical application of data cleaning, exploratory data analysis (EDA), feature engineering, machine learning modelling, and business insight reporting.


##  Project Structure

notebooks/      Jupyter Notebook (analysis + modelling)
reports/        Executive summary / business report
images/         EDA charts & visualizations
models/         Trained ML models 
data/           Dataset or dataset source link
README.md


##  Business Problem

Customer churn refers to customers who stop using the company’s services.

Churn matters because:
- retaining customers is cheaper than acquiring new ones
- churn reduces recurring revenue and lifetime value
- high churn signals customer dissatisfaction or switching behaviour

Target variable:
- Churn = Yes → customer left
- Churn = No  → customer retained

Project objectives:
- identify customers most likely to churn
- understand behavioural and contractual churn drivers
- build predictive churn models
- recommend strategies to reduce churn


##  Dataset Description

Rows: 7,043 customer records

Includes:
- demographics
- tenure and lifecycle stage
- internet and phone services
- contract type and billing method
- monthly and total charges
- churn status

Dataset Source:
IBM Telco Customer Churn Dataset (public dataset)


##  Data Cleaning & Preparation

Key steps:
- converted TotalCharges to numeric
- handled missing values for zero-tenure customers
- created binary churn label (Churn_flag)
- validated numerical and categorical fields

Dataset prepared for EDA and modelling.


##  Exploratory Data Analysis — Key Findings

Contract type strongly influences churn:
- Month-to-month → highest churn (~40%+)
- One-year → moderate churn
- Two-year → lowest churn

Tenure affects churn:
- highest churn in first 12 months
- churn decreases with longer tenure

Internet service impact:
- fiber-optic customers churn more than DSL users

Payment method impact:
- electronic check users churn more
- autopay users are more stable


##  Feature Engineering

Created features such as:
- tenure groups
- number of subscribed services
- lifecycle segmentation
- service engagement indicators

Improved model interpretability and prediction accuracy.


##  Machine Learning Models

Models trained:
- Logistic Regression
- Random Forest Classifier

Evaluation metrics:
- Accuracy
- Precision & Recall
- ROC-AUC
- Confusion Matrix

Final model:
Random Forest (chosen for higher churn recall)

Business reasoning:
Missing a churner has a higher cost than a false flag.


##  Post-Predictive Insights

High-risk churn segments include:
- month-to-month customers
- low-tenure customers
- fiber-optic users
- customers with high monthly charges

Some mid-tenure churners require additional behavioural data.


##  Business Recommendations

1) Transition month-to-month customers to 1-year plans  
2) Strengthen first-year onboarding and engagement  
3) Improve fiber-customer service experience  
4) Encourage migration to automatic payment methods  
5) Bundle value-added services to increase loyalty

Goals:
- reduce churn rate
- improve retention
- increase customer lifetime value


##  Future Improvements

Planned enhancements:
- behavioural churn analytics
- geographic churn segmentation
- survival / time-to-churn modelling
- Power BI or Tableau dashboard


##  Author

Mildred Okonye  
Data Analyst | Data Science Enthusiast
