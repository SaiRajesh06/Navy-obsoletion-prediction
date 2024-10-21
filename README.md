**Project Overview**
This project aims to predict device failure using time-series data consisting of voltage readings. The goal is to develop models that can forecast when a device will fail or estimate the risk of failure based on historical sensor data.

**Features & Approach**
**Data Processing:**
Applied a sliding window (size 10 or 20) to voltage data.
Computed 12 statistical metrics (e.g., mean, standard deviation, min/max) for both original voltage and delta voltage (successive differences between readings).
Combined these metrics with temperature data, resulting in a total of 25 features for each time window.
**Modeling:**
Developed predictive models using LSTM Autoencoders and other Deep Neural Networks (DNNs) to analyze the data.
The models addressed multiple prediction tasks:
**Binary Classification:** Predicting whether a device will fail during the experiment.
Risk Prediction: Estimating the risk of device failure over time.
**Technologies Used:**
Languages/Frameworks: Python, NumPy, Pandas, Scikit-learn, TensorFlow/Keras
Usage
**Data Preparation:**
Use the provided Python script to preprocess raw voltage and temperature data.
The script generates a time-windowed dataset with 25 features per row, suitable for model input.
Model Training:
Train the LSTM Autoencoder or other DNN models using the preprocessed dataset.
The model will predict failure or estimate the time to failure based on the given input.
**Prediction:**
Run the trained model on new device data to predict:
The risk of device failure.
Whether a device will fail soon (binary classification).
