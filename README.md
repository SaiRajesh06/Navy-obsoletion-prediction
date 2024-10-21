Project Overview
This project aims to predict device failure using time-series data consisting of temperature and voltage readings. The goal is to develop models that can identify when a device will fail or estimate the risk of failure based on historical sensor data.

Features & Approach
Data Processing:
Utilized a sliding window (size 10 or 20) on voltage data.
Computed 12 statistical metrics (e.g., mean, standard deviation) for both original voltage and delta voltage (successive differences).
Combined with temperature data to create a total of 25 features for each window.
Modeling:
Developed predictive models using LSTM Autoencoders and other Deep Neural Networks (DNNs).
Addressed multiple prediction tasks:
Predicting whether a device will fail during the experiment (binary classification).
Estimating the time until a device fails.
Predicting the risk of device failure over time.
Technologies Used: Python, NumPy, Pandas, Scikit-learn, TensorFlow/Keras.
Usage
Data Preparation: Use the provided Python script to convert raw voltage and temperature data into a time-windowed format with 25 features per row.
Model Training: Train the LSTM Autoencoder or other DNN models on the preprocessed dataset to predict device failure or estimate time to failure.
Prediction: Run the trained model to predict the failure risk for new devices or to classify imminent failure.
