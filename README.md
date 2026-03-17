# Bike Rental Demand Forecasting in Washington, DC

## Overview

This project analyzes daily bike rental demand in the Capital Bikeshare system in Washington, DC using historical data from 2011–2012. The objective is to identify demand patterns, explore seasonal behavior, and build time series forecasting models that can support operational planning and pricing decisions.

Understanding demand patterns helps bike-share operators maintain appropriate fleet levels, schedule maintenance efficiently, and improve overall system availability.

---

## Business Problem

Bike sharing systems must accurately forecast demand in order to manage fleet availability, station capacity, and operational costs. Reliable forecasts allow operators to determine how many bikes should be available at different times while also supporting pricing and maintenance planning.

This analysis uses historical Capital Bikeshare data to explore patterns in daily bike rental demand and develop forecasting models that can support operational decision-making.

---

## Dataset

The dataset contains daily counts of rental bikes in the Washington, DC Capital Bikeshare system during **2011–2012**, along with weather and seasonal variables.

**Source**

UCI Machine Learning Repository
Bike Sharing Dataset
https://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset

---

## Analysis Workflow

The project follows a standard data analytics and forecasting workflow:

1. **Data Preparation**

   * Load and inspect the dataset
   * Convert the data into a time-series structure

2. **Exploratory Data Analysis**

   * Analyze overall rental trends
   * Examine relationships between temperature and demand
   * Visualize seasonal patterns

3. **Trend and Seasonality Analysis**

   * Decompose the time series
   * Identify long-term trends and repeating seasonal components

4. **Model Development**

   * Naive forecasting model
   * Seasonal naive benchmark model
   * ARIMA forecasting model

5. **Model Evaluation**

   * Rolling cross-validation
   * Forecast accuracy comparison

6. **Forecast Generation**

   * Produce future demand forecasts
   * Visualize predicted rental demand

---

## Tools Used

* **R**
* tidyverse
* lubridate
* tsibble
* feasts
* fable
* tseries
* ggplot2

---

## Key Findings

* Bike rental demand exhibits **clear seasonal patterns**, with significantly higher usage during warmer months.
* **Temperature shows a strong positive relationship** with daily rental counts.
* The **ARIMA model outperforms naive benchmark models** in short-term forecasting accuracy.
* Forecasting models can support operational planning for bike availability, staffing, and maintenance.

---

## Business Recommendations

Based on the analysis:

* Increase fleet availability during **peak summer demand periods**.
* Schedule maintenance and system upgrades during **lower-demand winter months**.
* Use forecast outputs to support **staffing, bike redistribution, and operational planning**.
* Consider **weather-responsive pricing or promotions** to stabilize demand during transitional seasons.

---

## Limitations

* The dataset covers only **two years (2011–2012)** of historical data.
* The analysis uses **system-wide daily totals**, not station-level activity.
* Additional factors such as **precipitation, events, or pricing changes** were not included.

---

## Future Improvements

Possible extensions to the analysis include:

* Incorporating additional years of data
* Adding richer weather variables
* Building station-level forecasting models
* Comparing ARIMA models with other forecasting approaches such as ETS or machine learning methods

---

## Full Report

The complete analysis and forecasting report is available on RPubs:

https://rpubs.com/Nikki0686/bike-rental-demand-forecasting

---

## Author

**Nikki Carlson**
Data Analytics and Time Series Forecasting Project
2026
