# pyforesight
Enhanced Automatic time series forecasting using ARIMA family of models. 
Implements the basic Auto-ARIMA with additional functionalities in python creating a robust algorithm to handle any type of series for forecasting. 
Automatically chooses the best model for forecasting based on the model score.

Additional Features above the basic Auto-ARIMA implementation,
1. Automatically inferring time series frequency and seasonal period if not provided in input
2. Handling long seasonalities
3. Accepting Holiday feature to be used while model building
4. Power transformation for handling multiplicative series


Usage:

forecast <data_file_path_on_disk> <date_column_name> <time_series_column_name> <forecast_steps> ["FREQUENCY=<date_frequency>,SEASONAL_PERIOD=<seasonal_period>"]

FREQUENCY and SEASONAL_PERIOD are optional parameters.

Output after model training on the Air Passengers dataset
![Airlines Dataset example](docs/AirlinesForecast.png?raw=true "Airlines Data Forecasting")

Currently only csv data file type is supported.

Future scope:
1. Consider change-points in the time series to improve the forecasting accuracy.
2. Consider multiple seasonalities present in time series
