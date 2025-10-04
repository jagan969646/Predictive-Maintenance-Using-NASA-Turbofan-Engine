# Predictive-Maintenance-Using-NASA-Turbofan-Engine
This project applies predictive maintenance methods to the NASA CMAPSS dataset for estimating the Remaining Useful Life (RUL) of turbofan engines. Accurate RUL prediction is crucial in aerospace and industrial systems to avoid unexpected failures and reduce costs.
The dataset, containing multivariate time-series sensor data, was preprocessed through cleaning, normalization, and feature engineering. Rolling statistics (mean, standard deviation, slope) were generated to capture degradation trends. RUL values were derived by subtracting the operating cycle from the engine’s maximum cycle.

A baseline machine learning model (XGBoost) was trained on these features, achieving an RMSE of 31.4 and MAE of 22.6, providing a strong reference point.

Deep learning models were then developed:

LSTM (Long Short-Term Memory) networks were trained to learn sequential patterns in sensor data. Gradient clipping and early stopping improved stability.

CNN-LSTM hybrids were introduced to capture both local and long-term dependencies. While initial results showed instability, the architecture remains promising with further tuning.

Model performance was evaluated using RMSE, MAE, and visualizations of predicted versus actual RUL. Results showed that while XGBoost delivered reliable baseline performance, LSTMs and CNN-LSTMs demonstrated potential for improved long-term prediction.

The project highlights the importance of data preprocessing, normalization, and feature design in predictive maintenance. Future improvements include attention-based models or Transformers for more accurate and robust RUL estimation.

This work demonstrates how machine learning and deep learning can support predictive maintenance in aerospace and other industries, leading to improved safety, reduced downtime, and lower operational costs.
