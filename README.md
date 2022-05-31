# Multivariate-Solar-Radiation-Prediction
Multivariate Time-Series forecasting of Solar Radiation using RNN, LSTM and GRU.


# Neural networks based multivariate time series forecasting of solar radiation using meteorological data of different cities of Bangladesh

This repository is the official implementation of [Neural networks based multivariate time series forecasting of solar radiation using meteorological data of different cities of Bangladesh](https://www.sciencedirect.com/science/article/pii/S2590123022000354). 

## Data

<div style="text-align: justify"> Data for solar radiation was collected from the mentioned five cities. Taking a continuous reading is very expensive; the data was taken from 05:00 to 20:00 at fourteen intervals. Then we sum up all of the fourteen readings for the day. We could not collect data for every month of the year for all five cities. Knowing only solar radiation is not enough to predict future data. So, we collected data on other parameters from the Time and Date website. </div>

<div style="text-align: justify"> Dhaka (Latitude: 23.77, Longitude: 90.39) is the capital of the country, located in the center region of Bangladesh. Dhaka is the biggest city in Bangladesh, both in terms of population and area. Chuadanga (Latitude: 23.63, Longitude: 88.85) is located in the western part of the country, in the Khulna division. Bogra (Latitude: 24.84, Longitude: 89.37) and Dinajpur (Latitude: 25.63, Longitude: 88.63) are in the northern part of Bangladesh. Satkhira (Latitude: 22.72, Longitude: 89.07) is in the country's southwestern part and falls under the Khulna division. After cutting off the outliers, we have a total of 4036 entries. We have 812 entries for Bogra, 1064 entries for Chuadanga, 862 entries for Dhaka, 412 entries for Dinajpur, and 886 for Satkhira. </div>

|    **Parameter**    |               **Unit**               |
|:-------------------:|:------------------------------------:|
|      Unix Time      |             Second (sec)             |
|      Day Length     |             Second (sec)             |
| Maximum Temperature |          Degree Celsius (°C)         |
| Minimum Temperature |          Degree Celsius (°C)         |
|   Maximum Humidity  |            Percentage (%)            |
|   Minimum Humidity  |            Percentage (%)            |
|  Barometer Reading  |            Millibars (mb)            |
|      Wind Speed     |       Kilometer per hour (km/h)      |
|   Solar Radiation   | Kilo Watt per square meter (KWh/m−2) |

## Results

Performance comparison on different metrics:

| Model | MSE   | MAE   | RMSE  | MAPE(%) |
|-------|-------|-------|-------|---------|
| RNN   | 0.918 | 0.752 | 0.958 | 21.88   |
| LSTM  | 1.31  | 0.890 | 1.14  | 24.94   |
| GRU   | 0.795 | 0.682 | 0.891 | 19.28   |


Performance comparison by station:

| Station   | MSE   | MAE   | RMSE  | MAPE (%) |
|-----------|-------|-------|-------|----------|
| Dhaka     | 0.799 | 0.691 | 0.893 | 20.16    |
| Bogra     | 1.07  | 0.851 | 1.03  | 24.14    |
| Dinajpur  | 1.63  | 0.995 | 1.28  | 27.96    |
| Satkhira  | 0.559 | 0.586 | 0.747 | 16.50    |
| Chuadanga | 1.02  | 0.765 | 1.01  | 19.80    |
