# air-quality-forecasting
#Project Overview#
The goal of this project is to demonstrate a complete pipeline for time series forecasting, from data preprocessing to model deployment. It leverages Facebook's Prophet library for robust forecasting and Streamlit for creating an accessible and interactive user interface.

#Features#
1.Data Loading: Loads air quality data from a CSV file.
2.Data Preprocessing: Aggregates daily data to monthly averages and applies log-transformation for better model performance.
3.Prophet Model: Trains a Prophet model with yearly seasonality.
4.Interactive Forecasting: Allows users to select the number of future months for forecasting.
5.Visualization: Displays historical data and future forecasts with prediction intervals using interactive Plotly charts.

The project uses an air_quality_clean.csv dataset, which is expected to contain at least two columns: Date (datetime) and Air_Quality (numerical, representing air quality measurements).

#Model#
The forecasting model used is Prophet, an open-source forecasting library developed by Facebook. Prophet is designed for forecasting univariate time series with strong seasonal components. Key aspects of the model configuration include:

Yearly Seasonality: Enabled to capture recurring patterns over a year.

Daily Seasonality: Disabled, as the data is aggregated monthly.
