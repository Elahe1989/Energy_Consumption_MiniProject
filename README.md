Energy Consumption Mini‑Project
Machine Learning mini‑project for detecting high‑consumption periods using real sensor data.

This project explores a small energy‑consumption dataset and builds two machine‑learning models (Logistic Regression and Random Forest) to classify each time period as normal or high consumption.
The project includes data preparation, exploratory analysis, modeling, evaluation, and interpretation.
Project Overview
Modern smart‑industry environments rely on continuous monitoring of energy usage.
High consumption increases cost, reduces efficiency, and may indicate abnormal machine behavior.

This project demonstrates how simple sensor data can be used to detect high‑consumption periods with high accuracy.
Objectives
Explore patterns in active power, voltage, intensity, and sub‑metering

Build a binary classification model for high consumption

Evaluate performance using accuracy, confusion matrix, and ROC curve

Provide practical insights for smart‑industry use
Dataset
The dataset is a sample of the Individual Household Electric Power Consumption dataset from UCI.

Main Variables
Global_active_power — total active power (kW)

Global_intensity — current intensity (A)

Voltage — supply voltage (V)

Sub_metering_1 — kitchen appliances

Sub_metering_2 — laundry appliances

Sub_metering_3 — heating/cooling

Timestamp — measurement time
Methods
The workflow includes:

Data loading

Cleaning and preprocessing

Feature selection

Train/test split

Model training

Logistic Regression

Random Forest
Evaluation

Accuracy

Confusion Matrix

Classification Report

ROC Curve
Results
Logistic Regression
Accuracy: 99.35%

Very low false positives and false negatives

Strong performance with linear decision boundary

Random Forest
Accuracy: 100%

AUC = 1.00

Perfect separation of high vs. normal consumption

Random Forest slightly outperformed Logistic Regression due to its ability to capture non‑linear relationships.
Discussion
Strong correlation between active power and intensity explains high model performance.

Voltage shows negative correlation with load behavior.

Sub‑metering variables have weak correlations, indicating different appliance groups.

Perfect Random Forest performance may indicate overfitting due to small dataset size.
Limitations
Small dataset

No external features (temperature, machine status, production load)

Threshold for high consumption chosen manually

No time‑series modeling
Future Improvements
Use larger dataset

Add external variables

Apply time‑series models (LSTM, ARIMA)

Test additional ML models (XGBoost, Gradient Boosting)
Governance, Privacy & Security
Energy‑consumption data must be handled responsibly:

Protect sensor data from unauthorized access

Avoid monitoring individuals without consent

Apply clear data‑retention and access‑control policies

Ensure ethical use of ML predictions
Files in This Repository
energy_project.ipynb — main Colab notebook

energy_small.csv — dataset sample

README.md — project documentation
References
UCI Machine Learning Repository

Scikit‑Learn Documentation

Matplotlib Documentation

Seaborn Documentation
