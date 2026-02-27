✈️ Airline Revenue per ASK Prediction
📌 Project Overview

This project aims to predict Revenue per ASK (Available Seat Kilometer) using airline operational and efficiency-related features.

Revenue per ASK is a key airline industry metric that measures revenue generated per available seat kilometer and reflects pricing power and operational performance.

The project follows a complete machine learning workflow including data cleaning, leakage removal, feature engineering, model comparison, cross-validation, and residual analysis.

🎯 Problem Statement

To build a regression model that predicts Revenue per ASK based on airline operational and financial indicators such as:

Aircraft Utilization
Load Factor
Fleet Availability
Fuel Efficiency
Maintenance Downtime
Delay
Ancillary Revenue
Debt-to-Equity Ratio

📊 Dataset Description

The dataset contains 200,000 records with airline operational and financial metrics.

Target Variable: Revenue per ASK

Key Features:

Delay (Minutes)

Aircraft Utilization (Hours/Day)

Turnaround Time (Minutes)

Load Factor (%)

Fleet Availability (%)

Maintenance Downtime (Hours)

Fuel Efficiency (ASK)

Ancillary Revenue (USD)

Debt-to-Equity Ratio

🧹 Data Preprocessing

Checked for missing values (none found).
Removed identifier columns.
Removed data leakage columns:
Revenue (USD)
Operating Cost (USD)
Profit (USD)
Net Profit Margin (%)
Cost per ASK

Leakage removal ensured realistic model performance.

🧠 Feature Engineering

Created interaction-based features such as:
Operational Efficiency
Utilization per Downtime
Delay Impact Score
Revenue Capacity Index
Ancillary Ratio

These were designed to capture non-linear interactions between operational metrics.

🤖 Models Used

Linear Regression (Baseline)

Random Forest Regressor

XGBoost Regressor

📈 Model Performance
Model	R² Score
Linear Regression	~0.17
Random Forest	~0.16
XGBoost	~0.18

Cross-Validation (5-Fold):

Mean R²: ~0.177

Standard Deviation: ~0.001

The results indicate stable but limited predictive power.

🔍 Residual Analysis

Residual distribution centered around zero.

Residual plot showed heteroscedasticity (increasing error spread for higher predicted values).

No strong systematic bias observed.

📊 Feature Importance

XGBoost analysis showed:

Fuel Efficiency (ASK) is the dominant predictor.

Other features contribute minimally.

This suggests Revenue per ASK in this dataset is primarily driven by fuel efficiency.

🧠 Key Findings

Revenue per ASK shows weak correlation with most operational features.

Ensemble models did not significantly outperform linear regression.

Cross-validation confirmed model stability.

The dataset demonstrates limited predictive structure.

⚠ Limitations

The dataset appears partially synthetic.

Revenue per ASK may not strongly depend on available operational features.

Heteroscedasticity observed in residuals.

🚀 Future Improvements

Introduce additional pricing-related variables.

Apply advanced hyperparameter tuning.

Try classification-based modeling (e.g., High vs Low Revenue per ASK).

Use real-world airline datasets for stronger predictive power.

🛠 Tech Stack

Python

Pandas

NumPy

Scikit-learn

XGBoost

Matplotlib

Seaborn

▶ How To Run

Clone repository

Create virtual environment

Install dependencies:

pip install -r requirements.txt

Run Jupyter Notebook
