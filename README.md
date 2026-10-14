# Task 1: Weather Forecast API & Time-Series EDA

## Project Overview

This project focuses on weather data acquisition through a public weather API and exploratory time-series analysis of daily weather observations for Cairo, Egypt, covering the period from 2016 to 2025.

## Objectives

* Connect to a public weather API and collect weather data.
* Structure and prepare weather data for time-series analysis.
* Explore temperature trends and seasonal patterns.
* Test stationarity using the Augmented Dickey-Fuller (ADF) test.
* Analyze correlations between weather variables.
* Investigate wind speed, relative humidity, and precipitation distributions.
* Identify potential outliers for further investigation.

## Dataset

The dataset contains 3,653 daily observations covering the period from 2016 to 2025.

Weather variables analyzed include:

* Mean temperature
* Maximum temperature
* Minimum temperature
* Relative humidity
* Wind speed
* Precipitation

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Statsmodels
* Public Weather API
* Jupyter Notebook

## Key Findings

* STL decomposition revealed annual temperature seasonality.
* The ADF test returned a statistic of -4.2619 and a p-value of 0.000517, providing evidence against a unit root in the analyzed mean-temperature series.
* Mean temperature showed strong positive correlations with maximum temperature (0.988) and minimum temperature (0.978).
* Relative humidity had a negative correlation with mean temperature (-0.719).
* Approximately 74.57% of daily observations recorded zero precipitation.
* Potential outliers were identified for further validation.

## Project Structure

* `task4.ipynb`: Notebook containing data acquisition, preprocessing, visualizations, statistical tests, and exploratory analysis.
* `summary.md`: Summary of the main findings.
* `weather_data.csv`: Weather data in CSV format.
* `weather_data.json`: Weather data in JSON format.

*Note: Replace the example dataset filenames above with the actual filenames used in the repository.*

## Conclusion

This project demonstrates a time-series exploratory data analysis workflow, from weather data collection and preparation to visualization, statistical testing, and interpretation of temporal patterns and relationships between weather variables.

