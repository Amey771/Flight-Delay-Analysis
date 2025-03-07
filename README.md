# Scalable Databases – Final Project Phase 2

## Overview

This repository contains the final project (Phase 1 & 2) for the Scalable Databases course. The goal of the project is to analyze flight delay data using big data techniques and predictive modeling. The project spans from data sampling in Hive to advanced machine learning model implementation in Python, culminating in high-accuracy predictions of flight delays.

---

## Data Sampling in Hive

- **Sample Table Creation:** A new sample table was created in Hive.
- **Delayed Column:** A new column, "Delayed", was added to flag flight delays.
- **Random Sampling:** 30,000 rows were extracted using random sampling to create a manageable dataset.
- **Data Export:** The sample data was exported as a CSV file to be used in subsequent stages.

---

## Data Preparation in Python

1. **Data Merging:** Combined sample data across all years.
2. **Handling Missing Values:**  
   - Identified columns with null values.
   - Dropped columns with excessive missing data.
3. **Data Transformation:**  
   - Replaced missing numerical values with the median.
   - Replaced missing categorical values with the mode.
   - Encoded categorical variables using `LabelEncoder`.
4. **Data Splitting:** Divided the data into training, validation, and test sets.

---

## Model Implementation

Multiple machine learning models were implemented to predict flight delays:

- **XGBoost**
- **Gradient Boosting**
- **Decision Trees**
- **Random Forest**
- **Logistic Regression**

**Highlights:**
- The **XGBoost** model showed superior performance compared to other algorithms.

---

## Model Evaluations

- Models were assessed using various performance metrics.
- The XGBoost model achieved approximately **90% accuracy** on the test dataset.
- Detailed comparisons were made to determine the best-performing model for predicting flight delays.

---

## Target Predictions

- **Prediction Pipeline:** The final model was used to generate target predictions.
- **Delay Calculations:** Additional features (`depdelay` and `arrdelay`) were created by computing the differences between actual and scheduled times.
- The predictions provide actionable insights into potential flight delays based on input features.

---

## Conclusion

- The project successfully demonstrates an end-to-end data pipeline—from data extraction in Hive to predictive modeling in Python.
- **XGBoost** emerged as the best-performing model, delivering high accuracy in predicting flight delays.
- This work provides a scalable approach to handling large datasets and implementing machine learning solutions in a production-like environment.

---

## Extra Steps & Credits

- **Extra Verification:** An additional check was performed by calculating `depdelay` and `arrdelay` using actual versus scheduled times.
- **Team Effort:** Special thanks to all team members for their contributions and collaboration throughout the project.

---

Thank you for exploring our project! If you have any questions or feedback, please feel free to reach out.
