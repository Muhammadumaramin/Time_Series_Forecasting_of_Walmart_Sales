# Time Series Forecasting of Retail Sales Using ARIMA and ARIMAX Models: A Case Study of Walmart
This project explores Walmart’s historical weekly sales data to identify temporal patterns and build forecasting models using classical time series techniques. It applies ARIMA and ARIMAX models to predict future sales while analyzing the impact of external factors like fuel prices, unemployment rates, and holiday effects.

# Project Objectives:
> Understand the structure and seasonality of Walmart's weekly sales data
> Perform stationarity testing, autocorrelation analysis, and time series decomposition
> Develop ARIMA models for univariate forecasting
> Extend the model with exogenous regressors using ARIMAX
> Evaluate models using accuracy metrics and holdout validation
> Visualize actual vs. predicted performance

# Techniques:

> ARIMA, ARIMAX modeling
> ADF Test, ACF/PACF
> Ljung-Box Test
> Holdout evaluation

# Result: 
This project explored the forecasting of Walmart’s weekly sales using ARIMA and Linear Regression models. The dataset, after preprocessing and aggregation at the store level, was analyzed for temporal patterns. ARIMA modeling followed standard stationarity tests and ACF/PACF analysis, while Linear Regression was applied using store identifiers and dates as predictors. 
The ARIMA model achieved an RMSE of 1983.47, outperforming Linear Regression, which resulted in a significantly higher RMSE of 8768.09. This confirmed ARIMA’s strength in capturing autocorrelation and time-dependent structures, which Linear Regression inherently overlooks in univariate forecasting tasks. 
However, the Walmart dataset includes several exogenous variables—such as holidays, fuel prices, temperature, and unemployment that were not utilized in the current models. The absence of these features limited the forecasting accuracy, particularly in capturing sudden spikes or dips during specific events. This indicates that an ARIMAX model, which allows for the integration of such external regressors, would likely outperform both ARIMA and Linear Regression by 
accounting for these additional drivers of sales behavior. 
Therefore, while ARIMA proved to be more suitable than Linear Regression for this univariate forecasting task, the findings suggest that a shift towards ARIMAX could provide more robust and interpretable forecasts. Incorporating exogenous features into future models presents a promising direction for improving the accuracy and practical utility of sales predictions in retail environments. 
