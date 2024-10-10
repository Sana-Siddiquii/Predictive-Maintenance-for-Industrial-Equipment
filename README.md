# Predictive Maintenance for Industrial Equipment

This repository contains a predictive maintenance system designed to minimize equipment downtime using machine learning models. The project focuses on predicting machine failures based on historical data, enabling optimized maintenance schedules to prevent unexpected breakdowns.

## Project Overview
The primary objective of this project is to predict when industrial equipment is likely to fail, allowing for proactive maintenance. The system involves data preprocessing, feature engineering, and building machine learning models to identify failure patterns and recommend maintenance strategies.

### Dataset
The dataset includes the following features:
- **Machine ID**: A unique identifier for each machine.
- **Timestamp**: The date and time when the data was recorded.
- **Temperature**: The operating temperature of the machine (°C).
- **Pressure**: The pressure inside the machine (PSI).
- **Vibration**: The vibration level of the machine (mm/s).
- **Operational Hours**: The total number of hours the machine has been in operation.
- **Maintenance History**: Indicates whether the machine has undergone maintenance (Yes/No).
- **Failure**: Indicates whether the machine has failed (Yes/No).

### Models Used
Various machine learning models were trained and evaluated to predict machine failures:
1. **Random Forest Classifier**
2. **XGBoost Classifier**
3. **Support Vector Machine (SVM)**
4. **Gradient Boosting Classifier**
5. **Ensemble Model**: A combination of Gradient Boosting and XGBoost for improved performance.

### Results
The best-performing model was the **Support Vector Machine (SVM)**, with an accuracy of 0.60 and an F1-score of 0.67. An ensemble model combining **XGBoost** and **Gradient Boosting** achieved an accuracy of 0.91, providing more reliable predictions.

### Predictive Maintenance Strategy
Based on the models' predictions, the maintenance strategy was designed as follows:
- **Proactive Maintenance**: Machines with a failure probability higher than 70% are scheduled for immediate maintenance.
- **Scheduled Maintenance**: Machines with a failure probability between 40% and 70% are scheduled for maintenance during the next downtime period.
- **Routine Maintenance**: Machines with a failure probability lower than 40% continue on regular maintenance intervals.

---

### Files
- **`TASK_FINAL.ipynb`**: The Jupyter notebook containing the entire machine learning pipeline.
- **`Predictive_Maintenance_Report.pdf`**: A detailed report summarizing the project, data exploration, and results.

### Conclusion
The predictive maintenance models developed in this project demonstrate the potential to reduce equipment downtime by predicting machine failures in advance. By leveraging machine learning, industrial operations can optimize maintenance schedules and minimize unexpected breakdowns.

---
