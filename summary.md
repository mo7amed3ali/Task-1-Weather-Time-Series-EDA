# Task 4: Weather Forecast API & Time-Series EDA

## 1. Region and Time Period

This project analyzes daily weather observations for Cairo, Egypt, covering the period from 2016 to 2025. The dataset contains 3,653 daily observations and was obtained through a public weather API.

## 2. Data Source and Variables

Weather data was collected through the NASA POWER API. The analysis focuses on daily temperature variables, relative humidity, wind speed, and corrected precipitation. The data was structured as a time series and prepared for exploratory analysis.

## 3. Temporal Patterns and Seasonality

Time-series visualization and STL decomposition were used to investigate temperature trends and recurring seasonal patterns. The decomposition identified annual temperature seasonality, demonstrating recurring changes in temperature throughout the year.

## 4. Stationarity Analysis

The Augmented Dickey-Fuller (ADF) test returned a test statistic of -4.2619 and a p-value of 0.000517. Since the p-value is below 0.05, the null hypothesis of a unit root was rejected. This provides statistical evidence against a unit root in the analyzed daily mean temperature series. However, the result does not establish that all seasonal patterns have been removed.

## 5. Relationships Between Weather Variables

Correlation analysis identified strong positive relationships between mean temperature and maximum temperature (0.988), and between mean temperature and minimum temperature (0.978). Relative humidity showed a negative correlation with mean temperature (-0.719), while wind speed generally exhibited weaker correlations with the other analyzed variables.

## 6. Wind Speed and Relative Humidity

The mean wind speed was approximately 4.005 m/s, with a maximum recorded value of 10.33 m/s on March 13, 2020. The relative humidity averaged 52.686%, with values ranging from 12.12% to 88.72%. The IQR method identified one potential relative-humidity outlier, which should be investigated before considering any removal.

## 7. Precipitation Analysis

Of the 3,653 daily observations, 2,724 days (74.57%) had zero precipitation, while 929 days (25.43%) recorded positive precipitation. On rainy days, mean precipitation was 1.528 mm/day, compared with a median of 0.120 mm/day. This difference indicates a right-skewed distribution, with most rainy days receiving relatively little precipitation and a smaller number recording substantially higher amounts. The maximum recorded daily precipitation was 95.48 mm/day and may warrant further validation.

## 8. Conclusion

This exploratory analysis examined the temporal structure, seasonal behavior, statistical properties, and relationships among weather variables in Cairo from 2016 to 2025. The results highlight annual temperature seasonality, evidence against a unit root in the analyzed mean-temperature series, a negative association between temperature and relative humidity, and an uneven distribution of precipitation. Potential outliers should be validated against the source data rather than removed automatically. These findings provide a foundation for understanding the dataset and preparing it for subsequent time-series analysis.

