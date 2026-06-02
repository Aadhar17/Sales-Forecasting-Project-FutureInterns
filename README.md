# Sales Forecasting using Machine Learning

## Project Overview

This project predicts future sales using historical sales data from the Superstore dataset.

The objective is to build a machine learning pipeline capable of forecasting sales trends and identifying important factors influencing sales performance.

---

## Dataset

Dataset Used: Superstore Sales Dataset

Key Columns:

- Order Date
- Sales

After preprocessing, sales were aggregated to daily sales values.

---

## Project Workflow

### 1. Data Understanding

- Data cleaning
- Date conversion
- Daily sales aggregation
- Trend analysis
- Seasonality analysis

### 2. Feature Engineering

Created:

- Year
- Month
- Day
- Weekday
- Lag_1
- Lag_7
- Lag_30
- Rolling_7_Mean
- Rolling_30_Mean

### 3. Model Building

Models Used:

- Linear Regression
- Random Forest Regressor

Hyperparameter tuning performed using GridSearchCV.

### 4. Model Evaluation

Evaluation Metrics:

- MAE
- RMSE
- R² Score

Visualizations:

- Actual vs Predicted Sales
- Residual Analysis
- Feature Importance Analysis

### 5. Model Deployment

- Model saved using Joblib
- Model reloaded for future predictions

---

## Results

Best Model:
Random Forest Regressor

Performance:

- MAE ≈ 1690
- RMSE ≈ 2279
- R² ≈ 0.163

Most Important Features:

- Lag_30
- Lag_7
- Lag_1

---

## Key Insights

- Historical sales information was the strongest predictor of future sales.
- Feature engineering significantly improved performance.
- The model successfully captured overall sales trends.
- Extreme sales spikes remained difficult to predict.

---

## Future Improvements

- Holiday features
- Promotion and discount information
- Advanced forecasting models (XGBoost, Prophet, ARIMA)
- Dashboard deployment using Streamlit