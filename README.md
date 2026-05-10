# Predictive-maintenance-machine-learning
Machine learning project for predicting industrial machine failures using sensor and operational data.

## Project Overview
This project focuses on predicting machine failures using industrial sensors and operational data. Machine learning models were trained to identify high-risk machines based on temperature, rotational speed, torque, and tool wear measurements.

## Business Problem
Unexpected machine failures can lead to production downtime, maintenance costs, and operational inefficiencies. The objective of this project is to develop a predictive maintenance model capable of identifying machines likely to fail before breakdown occurs.

## Dataset Information
- Source: AI4I 2020 Predictive Maintenance Dataset
- Total Records: 10,000
- Failure Cases: 339
- Features:
  - Air Temperature
  - Process Temperature
  - Rotational Speed
  - Torque
  - Tool Wear
  - Machine Type
 
## Data Preprocessing
- Renamed columns for consistency
- Checked missing values and duplicates
- Handled categorical encoding
- Created engineered feature: `temp_difference`
- Removed leakage-related failure label columns

## Machine Learning Models
Models Used:
- Logistic Regression
- Random Forest Classifier

## Model Evaluation
Random Forest Performance:
- Accuracy: 98%
- ROC-AUC: 0.96
- High recall for machine failure detection

## Key Insights
- Only 3.39% of records represented machine failures, making the dataset highly imbalanced.
- Failed machines showed significantly higher average torque and tool wear.
- Torque, rotational speed, and tool wear were among the most influential features.
- Random Forest outperformed Logistic Regression in detecting machine failures.

## Business Impact
This model can support predictive maintenance strategies by helping maintenance teams detect high-risk machines earlier, reduce unexpected downtime, and improve maintenance scheduling efficiency.

## Technologies Used
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebook
