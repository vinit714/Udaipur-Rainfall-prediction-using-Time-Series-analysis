# Udaipur-Rainfall-prediction-using-Time-Series-analysis
In this project we see time series analysis Seasonal Autoregressive Integrated Moving Average (SARIMA) model to predict the rainfall in Udaipur district of Rajasthan, India.

# Problem Statement
This study carried out to Udaipur district of Rajasthan. Udaipur receives maximum rainfall due to the south-west monsoon in monsoon season and in all other seasons rainfall is very low for this area. Hence there is always a wide variation in daily annual rainfall as well as seasonal rainfall.

# Objective
Perform time series analysis Seasonal Autoregressive Integrated Moving Average (SARIMA) to predict the rainfall.

# Dataset
Rainfall data:
* Recorded monthly
* Measured in millimeters (mm)
* Starting Date : 01-01-2010
* End Date : 01-12-2020
* district : Udaipur

The dataset taken from knoema https://knoema.com/aulvzxc/district-wise-rainfall-data-for-india?regionId=IN-RJ

# Pipeline of the Project
* Clean the dataset
* Visualize the time series
* Stationarize the series
* Plot Autocorrelation and Partial Autocorrelation charts and find optimal parameters
* Build the SARIMA model
* Make prediction

![image](https://user-images.githubusercontent.com/52816788/138025365-59498404-c829-4f7d-83e8-dbddd1f0ea49.png)




# Seasonal Autoregressive Integrated Moving Average (SARIMA) model

Seasonal Autoregressive Integrated Moving Average, SARIMA or Seasonal ARIMA, is an extension of ARIMA that explicitly supports univariate time series data with a seasonal component.

It adds three new hyperparameters to specify the autoregression (AR), differencing (I) and moving average (MA) for the seasonal component of the series, as well as an additional parameter for the period of the seasonality.

# Output

We expect to predict rainfall of Udaipur of near future

# References


https://machinelearningmastery.com/sarima-for-time-series-forecasting-in-python/

https://becominghuman.ai/what-is-arima-and-sarima-model-10972b5e13c0

https://github.com/Ashwiniu07/Seasonal-Arima-Rain-Forecast.git




