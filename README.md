# AnalyticsProjects
A portfolio showing some of my projects in Business and Data Analytics.

# Project1: Forecasting China’s GDP using ARIMA modeling. 
https://github.com/NoelMga/AnalyticsProjects/blob/fcb2d2e42b2b0e22044a19d5388697e3f66e13b8/Forecast_CNA_ARIMA.R

Project Overview
In this project, we aim to forecast China’s Gross Domestic Product (GDP) using ARIMA (AutoRegressive Integrated Moving Average) modeling. We’ll walk through the steps involved in data preparation, model fitting, and visualization.

Steps Taken:
Data Loading and Preprocessing:
The dataset (CNAGDP.csv) was read into R.
The DATE column was transformed into a Date format.
The data was converted into a tsibble object with the key variable as MKTGDPCNA646NWDB.
Data Visualization:
A time series plot was created to visualize China’s GDP over time.
The plot shows the trend and any potential seasonality.
Autocorrelation Function (ACF) Analysis:
The ACF plot was generated to assess the correlation between GDP values at different lags.
If the ACF values are within a certain range (e.g., < 0.2), it suggests weak stationarity.
Modeling:
Exponential Smoothing (ETS):
An ETS model was fitted to the GDP data.
A one-step-ahead forecast was generated using the ETS model.
Auto-ARIMA:
An Auto-ARIMA model was fitted to the GDP data.
Another one-step-ahead forecast was generated using the Auto-ARIMA model.
Key Findings:
The ACF suggests weak stationarity, indicating that the GDP series may exhibit some seasonality.
The ETS and Auto-ARIMA models provide forecasts for the next time point.
Next Steps:
Consider evaluating model performance using appropriate metrics (e.g., Mean Absolute Error, Root Mean Squared Error).
Explore additional features or external factors that could improve forecasting accuracy.
