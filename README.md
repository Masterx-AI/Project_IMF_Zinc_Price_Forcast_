# AI/ML Project: IMF-Zinc Price Forecast 🪙

<p align="center"><img src="https://user-images.githubusercontent.com/54996245/144306851-055524e7-ab4f-4cef-8563-b4f6c70d6313.jpg" style="width: 1000px;"/></p>

### Description:

A simple yet challenging project, to forecast the IMF commodity price of Zinc, based on monthly totals zinc price recorded from 1980 to 2016.
Can you overcome these obstacles & Forecast the it's future prices?

**This data frame contains the following columns:**

* Month : The month of observation
* Price : Average Prices of zinc in that particular month

**Source:**

This dataset is taken from an inbuilt dataset of R called IMF-commodity-zinc.<br>

### Objectives:
- Understand the Dataset & cleanup (if required).
- Perform the necessary checks like stationarity & DF on the Dataset.
- Build a forcasting model to forecast Zinc prices.

### The Project is divided into the following steps:
1. Visualize the time series - Check for trend, seasonality, or random patterns.
2. Stationarize the series using decomposition or differencing techniques.
3. Plot ACF/PACF and find (p,d,q) parameters.
4. Building the forecasting model - can be AR, MA, ARMA or ARIMA.
5. Making Predictions using the Forecasting Model

### Some Visuals of the Project:

**1. Time-Series Data**
<p align="left"><img src="https://user-images.githubusercontent.com/54996245/144307036-076b843d-4e23-488e-928d-3ddc5713172c.png" /></p>

**2. Stationarity Check**

![image](https://user-images.githubusercontent.com/54996245/144307054-6e41f23e-7c7e-4f39-8df5-0e3422bbe826.png)

**3. Decomposing using moving average**

![image](https://user-images.githubusercontent.com/54996245/144307123-e1c6fd26-9d13-422b-bfa4-aa01c1bebcb1.png)

**4. Stationarity Check for Decomposed data**

![image](https://user-images.githubusercontent.com/54996245/144307133-d3e03aa8-c810-4abd-bc20-facb17078328.png)

**5. Auto Correlation Function Plot**

![image](https://user-images.githubusercontent.com/54996245/144307147-e9a74f39-8104-49a6-9f8a-61e8650cf590.png)

**6. Partial Auto Correlation Function Plot**

![image](https://user-images.githubusercontent.com/54996245/144307156-30e173b6-91e9-451a-9fc3-d22a0d95c87f.png)

**7. ARIMA Model Forecast**

![image](https://user-images.githubusercontent.com/54996245/144307169-448290e2-ce7e-4e1e-b320-067cb15e0a16.png)


### Here are some of the key outcomes of the project:
- The Zinc Price Time-Series Dataset was quiet small, with just 434 samples.
- It was clear from the visuals that the time-series dataset had an upward trend & some seasonality.
- The same was confirmed with help of visual (rolling mean & std) & statistical (Dicky-Fuller Test) stionarity checks.
- The time-series was subject to Decomposition in order to stationarize the outputs.
- Futher ACF & PACF curves were plotted to extract the values of p & q, as it is required for the ARIMA Model.
- The Forecasting Model was then built with the time-series data, by feeding the optimal p,q,d values.
- Finally, the model was used to forecast the time-series of the zinc prices, into the future.

