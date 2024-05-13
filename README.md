# Schuster_Payment_Analysis
Problem Statement
Background: Schuster is a multinational retail company dealing in sports goods, engaging in frequent credit transactions with various vendors. Not all vendors comply with their credit terms, leading to operational inefficiencies due to late payments.

Objective: To develop a predictive model to estimate the likelihood of late payments for open invoices, helping prioritize collection efforts, enhance payment compliance, and sustain business relationships.

Data Description
Received Payments Data: Detailed historical transactions including payment terms, dates, amounts, and customer specifics.
Open Invoices Data: Current invoices with incomplete payments, critical for understanding and predicting future payment behaviors.
Tasks and Methods
Data Preparation
Data Cleaning: Rigorous cleaning and preprocessing of datasets to remove inconsistencies and ensure data integrity.
Target Variable: Creation of a binary target variable 'Payment_Status', with 1 representing late payments and 0 for on-time payments, derived from the historical payment data.
Feature Engineering
Payment Terms Numeric Conversion: Textual payment terms were quantified to facilitate computational analysis, transforming terms like "Net 30" into a numerical value representing the number of days.
Customer Metrics: Developed metrics such as 'Average_Payment_Time' and 'Payment_Time_Variance' for each customer based on historical payment data. These metrics provide insights into each customer’s typical payment behavior.
Model Development
Feature Selection: Utilized techniques like Recursive Feature Elimination to identify the most predictive features for late payments.
Model Building: Tested various classification models including Logistic Regression, Decision Trees, Random Forests, and Gradient Boosting Machines to find the optimal model for predicting late payments.
Model Evaluation: Employed metrics such as accuracy, precision, recall, F1-score, and ROC-AUC to evaluate model performance. Model tuning was performed using grid search to optimize parameters for best results.
Key Findings
Insights: The analysis revealed specific patterns and predictors of late payments, such as the impact of payment term length and historical payment behavior on the likelihood of late payments.
Best Model: The Random Forest model outperformed others in terms of precision and recall, particularly effective in minimizing false negatives, which is critical for financial risk mitigation.
