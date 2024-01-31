# Time-series-forecasting-using-Prophet

![image](https://github.com/FeresDarouich/Time-series-forecasting-using-Prophet/assets/120333973/0d6838bf-b9f9-4239-9ad8-8d5e2fe6f31a)

Prophet is a forecasting tool developed by Facebook for time series data, and it is designed to handle data with strong seasonal patterns and multiple seasonality. Here is a high-level overview of how the Prophet model works:

* Additive Decomposition:

Prophet decomposes the time series into three main components: trend, seasonality, and holidays. The observed time series is assumed to be the sum of these components.
- Trend Component:

The trend component captures the overall direction (upward or downward) of the time series. It can be modeled as either linear or logistic growth.


- Seasonality Component:

Prophet incorporates both weekly and yearly seasonality by default. Weekly seasonality captures patterns that repeat every seven days, and yearly seasonality captures annual patterns.


- Holiday Effects:

Holidays and special events can significantly impact time series data. 

* Uncertainty Intervals:

Prophet provides uncertainty intervals for the forecasted values. It uses a Bayesian approach with Markov Chain Monte Carlo (MCMC) methods to estimate the uncertainty in the forecast.


* Automatic Changepoints:

Prophet automatically identifies potential changepoints in the time series data where the trajectory of the time series may change. These changepoints contribute to the flexibility of the model.


* parametres:

- growth: Specifies the type of growth for the time series. It can be 'linear' or 'logistic', depending on whether the data is expected to grow linearly or logistically. Linear growth , implies that the time series is expected to grow or decrease at a constant rate over time. The forecasted values follow a straight-line trajectory, indicating a steady and linear trend in the data. The logistic growth, implies that the time series is expected to approach a maximum limit or capacity over time.
The logistic growth model is often used when the growth of the time series is expected to slow down and eventually reach a saturation point. It is suitable for situations where there are limiting factors to growth.

- changepoints: Indicates the dates where the time series has potential changepoints. These are the points where the time series exhibits a shift in its trajectory.

- changepoint_prior_scale: Controls the flexibility of the changepoints. A higher value makes the trend more flexible and may result in more changepoints.

- seasonality: Specifies the seasonality components. It can be set to include weekly and yearly seasonality.

- seasonality_prior_scale: Controls the strength of the seasonality components.

- holidays: Allows the inclusion of holidays and special events that might impact the time series.

- interval_width: Sets the uncertainty interval for the forecast.

- mcmc_samples: If uncertainty intervals are specified, this parameter sets the number of MCMC (Markov Chain Monte Carlo) samples used to estimate uncertainty.
















