# Product-Sales-Forecasting-using-Time-Series-Analysis-


## Brief Summary
•Conducted ADFuller test for data stationarity, performed Data Decomposition to observe level, trend, seasonality & residue

•Implemented Seasonal ARIMA, Holt’s winter, and Prophet models on product sales dataset for Forecasting future sales 

•Observed SARIMA to yield the best performance among others with least RMSE of 8 & MAPE of 6 % errors respectively 


## Introduction 
Time Series Analysis is the most widely used field of data science and machine learning, it decomposes the past historical data to depict the trend, seasonality, and noise to derive the future trends from it. It’s a type of predictive analysis that forecasts the value of a variable in future occurrences based on history. The predicted values can be influenced by certain external factors which are known as independent variables like in the case of sale of a product is influenced by the discount percentage on its prices or the temperature on a particular day is influenced by the humidity or wind speed etc.

There are a number of time series forecasting algorithms available to a data scientist but the choice of algorithm depends on the business problems and the data set at hand. From simple time series forecasting techniques like moving average, exponential smoothing, ARIMA, etc to deep learning forecasting methods like recurrent neural networks, long short term memory, XG Boost, gradient boosting, fuzzy time series algorithms, etc can be used for analysis.

In this project we will try to forecast a time series data basically. We'll build three different model with Python and inspect their results. Models we will use are ARIMA (Autoregressive Integrated Moving Average), Holt's Winter and Facebook Prophet.

## Models:
## 1. Seasonal ARIMA (Seasonal Autoregressive Integrated Moving Average)
SARIMA is a model which is used for predicting future trends on a time series data. It is model that form of regression analysis.

AR (Autoregression) : Model that shows a changing variable that regresses on its own lagged/prior values.
I (Integrated) : Differencing of raw observations to allow for the time series to become stationary
MA (Moving average) : Dependency between an observation and a residual error from a moving average model
For ARIMA models, a standard notation would be ARIMA with p, d, and q, where integer values substitute for the parameters to indicate the type of ARIMA model used.

p: the number of lag observations in the model; also known as the lag order.
d: the number of times that the raw observations are differenced; also known as the degree of differencing.
q: the size of the moving average window; also known as the order of the moving average.

## 2. Holts Winters
Holt winter's method is one of the many time series prediction methods which can be used for forecasting time series data. The Holt-Winters forecasting algorithm allows users to smooth a time series and use that data to forecast areas of interest. Exponential smoothing assigns exponentially decreasing weights and values against historical data to decrease the value of the weight for the older data.

## 3. Prophet
Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.

## Results:
The analysis metrics used to compare the performance of above three models are RMSE, MSE, MAPE. The values of these metrics are obtained as below:

Models	     RMSE Errors	MSE Errors	MAPE Errors
ARIMA	       8.127305	    66.053093	  5.726577
HOLT WINTER	 12.781636	  163.370221	6.795875
Prophet	     11.428533	  130.611358	7.020210


## Conclusion:
Thus, on the basis of these results, the SARIMA model is more efficient in predicting the sales of products than the Holts Winter or Prophet model. In this study, we looked at forecasting product sales in every next month using the time series model.
