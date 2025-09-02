💳 Credit Card Consumption Prediction

This project focuses on predicting missing credit card consumption values (cc_cons) for banking customers using their demographic and behavioral data. It covers the complete pipeline of data preprocessing, feature engineering, model training, and evaluation.

✅ Problem Definition
The dataset consists of 20,000 customers:
15,000 customers → cc_cons (credit card consumption) is available.
5,000 customers → cc_cons is missing.

🎯 Objective: Build a machine learning model to predict the missing cc_cons values with high accuracy.

📊 Dataset Overview
CustomerDemographics.xlsx → Age, gender, income, tenure, etc.
CustomerBehaviorData.xlsx → Transaction history (3 months), card limits, loans, investments.
CreditConsumptionData.xlsx → Target variable cc_cons for training customers.

🔁 Project Workflow

Data Preprocessing
Combined all three datasets using Customer_ID.
Handled missing values through imputation.
Converted categorical variables into numeric format using one-hot encoding.

Model Building

Data split into training and validation sets.
Multiple algorithms tested:

✅ Linear Regression (best performing)
Random Forest Regressor
Gradient Boosting Regressor

Model Evaluation
Metrics used: MAE, MSE, RMSE, R², RMSPE
Linear Regression delivered the best balance of error rate and interpretability.

Prediction & Deployment

Used the final model to predict cc_cons for 5,000 customers with missing values.
Saved results into a structured output file.

🧪 Model Performance
| Model                       | MAE     | RMSE    | R²     | RMSPE  |
| --------------------------- | ------- | ------- | ------ | ------ |
| **Linear Regression**       | 1857.26 | 2577.96 | 0.8660 | 0.2703 |
| Random Forest Regressor     | 1942.74 | 2875.87 | 0.8332 | 0.2908 |
| Gradient Boosting Regressor | 1874.71 | 2674.19 | 0.8558 | 0.2852 |

📌 Linear Regression was finalized as the best model.

📁 Deliverables

predicted_credit_consumption_for_missing.csv → Predicted values for 5,000 customers.
results_report.md → Comparison of models with evaluation metrics.
Notebooks & Visualizations → Correlation heatmaps, feature importance plots, and exploratory analysis.

📌 Key Highlights

Complete handling of missing data using statistical imputation.
One-hot encoding applied for categorical features.
Feature selection guided by both correlation analysis and business understanding.
Achieved strong accuracy with Linear Regression (R² = 0.866).

⚡ This project demonstrates end-to-end data science workflow from raw data cleaning to delivering a final predictive model.
