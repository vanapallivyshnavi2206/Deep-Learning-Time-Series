# Deep Learning Time Series
## Research Internship at IIT Madras (May - July 2026)

This repository contains the work carried out during my Summer Research Internship at the **Department of Mathematics, IIT Madras**, under the guidance of **Prof. S. Sundar**.

The internship focuses on understanding and implementing statistical and deep learning models for time series forecasting. This repository includes the datasets, implementation notebooks, reports, presentations, and reference materials developed throughout the internship.



## Models Implemented

### 01. AutoRegressive (AR) & AutoRegressive Moving Average (ARMA)
- Explored the traffic volume dataset through **Exploratory Data Analysis (EDA)**, identifying missing timestamps and continuity gaps.
- Investigated time series characteristics using **Autocorrelation Function (ACF)** and **Partial Autocorrelation Function (PACF)**.
- Implemented the **Yule-Walker Equations** and **Maximum Likelihood Estimation (MLE)** for AR model parameter estimation.
- Validated the AR model through **causality, stationarity, and residual diagnostic analysis**, motivating the transition to **ARIMA and SARIMA** models.



### 02. AutoRegressive Integrated Moving Average (ARIMA) & Seasonal AutoRegressive Integrated Moving Average (SARIMA)
- Appiled **first-order** and **seasonal differencing** to transform the series into a stationary process.
- Developed **ARIMA** and **SARIMA** forecasting models, with model selection performed through **grid search**.
- Evaluated seasonal patterns and optimized model parameters using statistical model selection techniques.
- Validated the final SARIMA model through **residual diagnostics** and the **Ljung-Box test** to assess the independence of residuals.


### 03. AutoRegressive Neural Network (ARNN)
- Constructed autoregressive input matrices through **lag feature engineering** and optimized the network input configuration.
- Implemented the complete neural network learning pipeline, including **forward propagation, backpropagation, loss computation, and gradient descent optimization**.
- Trained and validated the ARNN model using **normalized data**, followed by forecasting and performance evaluation through **RMSE** and **MAE**.
- Investigated the learning behavior of the network through **loss convergence**, prediction analysis, and model testing on unseen time series data.



### 04. Probabilistic AutoRegressive Neural Network (PARNN)
- Integrated **ARIMA residuals** with lagged observations to capture both linear and nonlinear patterns within a unified forecasting framework.
- Determined the optimal network architecture by selecting the lag orders *(m, l)* and hidden neurons *(k)* using validation-based hyperparameter tuning.
- Produced **probabilistic forecasts** by aggregating predictions from multiple neural network initializations, improving forecast stability.
- Generated **multi-step ahead forecasts** through recursive prediction with uncertainty estimation.
