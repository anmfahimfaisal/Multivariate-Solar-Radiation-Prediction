# Multivariate-Solar-Radiation-Prediction
Multivariate Time-Series forecasting of Solar Radiation using RNN, LSTM and GRU.


# Neural networks based multivariate time series forecasting of solar radiation using meteorological data of different cities of Bangladesh

This repository is the official implementation of [Neural networks based multivariate time series forecasting of solar radiation using meteorological data of different cities of Bangladesh](https://www.sciencedirect.com/science/article/pii/S2590123022000354). 

## Results

Performance comparison on different metrics

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
