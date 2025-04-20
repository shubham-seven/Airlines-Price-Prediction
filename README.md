# Airlines-Price-Prediction
This model predicts the price based on given dataset on kaggle.

# ✈️ Hackathon Airlines Flight Price Prediction

This project was built as part of a Data Science hackathon challenge. The goal was to predict the **flight ticket price** based on various flight-related features using regression techniques and hyperparameter tuning.


## 📌 Problem Statement

Airlines operate in a highly competitive environment where optimizing ticket pricing is critical. The objective of this project is to build a machine learning model that accurately predicts **flight prices** using historical flight data including schedule, route, airline, and duration-related features.


## 📊 Dataset

- The dataset contains features like:
  - Airline
  - Source and Destination
  - Departure and Arrival Time
  - Duration
  - Total Stops
  - Additional Information

- **Target Variable**: `Price` (Numerical - continuous)


## 🛠️ Tools & Technologies

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- RandomizedSearchCV (for hyperparameter tuning)


## 🚀 Model Training & Tuning

- Used **XGBoost Regressor** to model flight prices
- Applied **RandomizedSearchCV** for efficient hyperparameter optimization
- Evaluation Metrics:
  - R² Score
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)

## 📈 Performance Metrics

| Metric | Value |
XGBoost Tuned Performance:
R2 Score: 0.9998043913411181
MAE: 196.72679485837867
RMSE: 253.47627684680916

