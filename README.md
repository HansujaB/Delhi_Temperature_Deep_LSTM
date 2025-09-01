Delhi Temperature Prediction using LSTM
This project uses a Long Short-Term Memory (LSTM) neural network to predict the mean daily temperature in Delhi, India. The model is trained on historical climate data and is designed to forecast the temperature for a single day based on a sequence of the previous 30 days.

Project Overview
The core of this project is a time-series forecasting model built with TensorFlow/Keras. The process involves:

Data Loading and Cleaning: Reading daily climate data from a CSV file, handling missing values, and removing outliers.

Feature Scaling: Normalizing the input features (mean temperature, humidity, wind speed, and mean pressure) using MinMaxScaler.

Data Preparation for LSTM: Structuring the data into sequences, where each sequence consists of 30 days of data used to predict the temperature of the 31st day.

Model Training: A Sequential model with multiple LSTM layers is trained on the prepared data.

Prediction and Evaluation: The trained model is used to make predictions on unseen test data, and its performance is evaluated using metrics like R-squared (R 
2
 ), Mean Absolute Error (MAE), and Mean Squared Error (MSE).

 Key Findings
The model can successfully learn patterns from the historical climate data.

The use of LSTMs is effective for this type of time-series forecasting problem.

Data preprocessing, including handling outliers and proper data scaling, is crucial for good model performance.
