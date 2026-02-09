# Household Energy Consumption Forecasting

## Project Overview
This project focuses on short-term household electricity consumption forecasting using machine learning techniques. A leakage-aware time-series forecasting pipeline is developed to ensure realistic and interpretable performance evaluation.

## Dataset
- Individual Household Electric Power Consumption Dataset
- Source: UCI Machine Learning Repository / Kaggle
- Data frequency: Minute-level, resampled to hourly
- Note: Dataset is publicly available and not included in this repository.

## Methodology
- Missing value handling using forward fill
- Temporal resampling from minute-level to hourly data
- Feature engineering:
  - Lag features (1, 24, 168 hours)
  - Rolling statistics
  - Time-based features (hour, day, month)
  - Peak-hour indicator
- Leakage prevention by removing sensor-derived variables
- Chronological train–test split

## Models Implemented
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

## Evaluation Metrics
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

## Results
Tree-based ensemble models achieved the best performance, with realistic R² values in the range of 0.51–0.60, indicating leakage-free forecasting under real-world constraints.

## How to Run
1. Clone the repository
2. Install dependencies using `requirements.txt`
3. Download the dataset from UCI/Kaggle
4. Run the notebook or Python script

## Author
[Geethu Satheesh]
