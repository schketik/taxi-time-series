
# Taxi Orders Prediction - Time Series Project

This project focuses on predicting the number of taxi orders for the next hour using historical data. The objective is to assist taxi companies in managing peak demand periods by providing accurate forecasts. The project includes the following steps:

### Project Overview:
1. **Data Resampling:** Data is resampled to an hourly frequency for consistency.
2. **Feature Engineering:** Creation of time-based features like day, hour, day of the week, and whether it's a weekend.
3. **Modeling:** Various machine learning models (Linear Regression, LightGBM, etc.) are trained with hyperparameter tuning to minimize **RMSE**.
4. **Seasonality Analysis:** Daily and weekly seasonality is analyzed to capture recurring patterns in taxi orders.

### Key Steps:
1. **Data Preparation:**
   - Data loaded and resampled by hour.
   - Missing values handled and time-based features extracted.
   
2. **Modeling:**
   - Multiple models were trained and evaluated, with **LightGBM** showing the best results based on RMSE.
   - Models trained with hyperparameters to predict future taxi orders for the next hour.

3. **Evaluation Metrics:**
   - The primary evaluation metric was **Root Mean Square Error (RMSE)**.
   - The goal was to achieve an RMSE of less than **48** on the test set.

4. **Results:**
   - **LightGBM** model provided the most accurate predictions, with minor difficulties in capturing peak values.

### Project Files:
- `taxi_orders_prediction.ipynb`: Main notebook with data exploration, modeling, and evaluation.
- `taxi.csv`: Dataset containing historical taxi order data.

### How to Run:
1. Clone the repository.
2. Install dependencies from `requirements.txt`.
3. Run the notebook to reproduce results.

### Conclusion:
The project demonstrates a successful time series forecasting model for predicting hourly taxi orders, providing useful insights into demand peaks for improved resource management.

