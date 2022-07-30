# Seoul-Bike-Sharing-Demand-Prediction

## Problem Description:
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.
# Data Description:

The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

# Attribute Information -

Date : year-month-day
Rented Bike count - Count of bikes rented at each hour
Hour - Hour of he day
Temperature-Temperature in Celsius
Humidity - %
Windspeed - m/s
Visibility - 10m
Dew point temperature - Celsius
Solar radiation - MJ/m2
Rainfall - mm
Snowfall - cm
Seasons - Winter, Spring, Summer, Autumn
Holiday - Holiday/No holiday
Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)
# Conclusion -
1.Most number of bikes are rented during evening time.

2.In summer more number of bikes are rented whereas, winter has the lowest count.
3.Least numbers of bike are rented on 12th of the month.

4.More bikes are rented if the humidity is low and wind-speed is high.

5.Rainfall and snowfall impact the number of bikes rented tremendously with very high downfall.

6.Linear regression is not suitable for our problem as it makes many assumptions and our dataset is prone to it. Thus, linear regression gives us the lowest r2-score and highest rmse.

7.Random forest regressor performs really good when compared to linear regression with high model performance and low rmse. But it's performance is low when compared to gradient boosting regressor. However, time taken for hyperparameter tuning and training the model is much low for random forest regressor then gradient boosting regressor. Thus, there's a tradeoff of accuracy and time in between random forest and gradient boosting regressor. It's up to us and business domain to which
algorithm to use.

8.Hour, temperature and solar radiation were the most important features for predicting the count of bikes required.
