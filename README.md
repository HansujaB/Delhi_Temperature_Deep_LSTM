# 🌡️ Delhi Temperature Prediction using LSTM

This project applies a **Long Short-Term Memory (LSTM)** neural network to predict the **mean daily temperature** in Delhi, India.  
The model learns from **historical climate data** and forecasts the temperature for a given day based on the **previous 30 days**.

---

## 📌 Project Overview

The workflow of this project involves the following steps:

### 🔹 Data Loading & Cleaning
- Load daily climate data from **CSV**.  
- Handle **missing values**.  
- Detect and remove **outliers** for better training.  

### 🔹 Feature Scaling
- Normalize input features:  
  - Mean Temperature  
  - Humidity  
  - Wind Speed  
  - Mean Pressure  
- Scaling done using **MinMaxScaler**.  

### 🔹 Data Preparation for LSTM
- Create **sequences of 30 days** of data to predict the **31st day temperature**.  

### 🔹 Model Training
- Build a **Sequential model** with **stacked LSTM layers** using **TensorFlow/Keras**.  
- Train the model on **preprocessed time-series data**.  

### 🔹 Prediction & Evaluation
- Generate **temperature predictions** on unseen test data.  
- Evaluate performance using:  
  - **R-squared (R²)**  
  - **Mean Absolute Error (MAE)**  
  - **Mean Squared Error (MSE)**  

---

## 🔑 Key Findings
- The model can **successfully learn patterns** from Delhi’s historical climate data.  
- **LSTMs** are well-suited for **time-series forecasting problems** like temperature prediction.  
- **Preprocessing steps** (handling outliers & scaling) are crucial for achieving better accuracy.  

---

## 🛠️ Tech Stack
- **Python 3**  
- **TensorFlow / Keras** (Deep Learning framework)  
- **NumPy & Pandas** (Data manipulation)  
- **Matplotlib / Seaborn** (Visualization)  
- **scikit-learn** (Scaling & metrics)  

---

## 📊 Results
- The trained LSTM achieved **good performance** in predicting Delhi’s mean temperature.  
- Model evaluation metrics (**R², MAE, MSE**) show that the network captures **seasonal and short-term trends effectively**.  
- Visualization of **actual vs predicted values** confirms the model’s predictive capability.  
