# Customer Churn Prediction Project

## Project Overview

This project focuses on predicting whether a customer is likely to churn or stay with an ecommerce platform. Churn refers to customers who stop purchasing or become inactive. The goal is to identify such customers early so that businesses can take retention actions and reduce revenue loss.

The project follows a complete machine learning workflow starting from raw data processing to model evaluation and prediction.

---

## Problem Statement

Customer retention is critical for ecommerce businesses. Acquiring new customers is expensive compared to retaining existing ones. This project aims to build a machine learning model that predicts customer churn based on historical customer behavior and engagement data.

---

## Dataset Description

The dataset contains historical ecommerce customer data where

* Each row represents a single customer
* Each column represents a customer attribute or behavior

The target column is **Churned**

* 1 indicates the customer has churned
* 0 indicates the customer is still active

The dataset includes information such as customer demographics, purchase behavior, engagement metrics and support interactions.

---

## Project Pipeline

1. Data Loading
   The dataset is loaded from a CSV file using pandas.

2. Data Inspection
   The structure, data types, missing values and duplicates are analyzed.

3. Data Cleaning

   * Duplicate records are removed
   * Missing values are handled using median and mode strategies
   * Invalid values are corrected
   * Target column consistency is ensured

4. Exploratory Data Analysis

   * Churn distribution is analyzed
   * Key behavioral patterns between churned and retained customers are visualized using matplotlib

5. Feature Engineering

   * Target and features are separated
   * Categorical variables are encoded
   * Numerical features are scaled
   * Data is split into training and testing sets

6. Model Training

   * Logistic Regression is used as a baseline model
   * Random Forest is used as the final model for better performance

7. Model Evaluation

   * Accuracy, precision, recall and F1 score are calculated
   * Confusion matrix is analyzed
   * Focus is placed on recall for churned customers

8. Model Interpretation

   * Feature importance is analyzed to understand key churn drivers

9. Prediction

   * The trained model is used to predict churn for new customer data

---

## Models Used

* Logistic Regression
  Used as a baseline to understand initial performance.

* Random Forest Classifier
  Selected as the final model due to significantly better recall and overall performance for churn prediction.

---

## Results Summary

* Logistic Regression achieved moderate accuracy but low recall for churned customers.
* Random Forest significantly improved churn recall and overall accuracy.
* Key churn influencing features include customer service calls, lifetime value, cart abandonment rate and customer engagement metrics.

---

## Feature Importance Insights

The model identified the most influential factors affecting churn such as

* Customer service interactions
* Customer lifetime value
* Cart abandonment behavior
* Purchase inactivity
* Engagement with emails and the platform

These insights can help businesses design targeted retention strategies.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

---

## How to Run the Project

1. Clone the repository
2. Create and activate a virtual environment
3. Install required dependencies
4. Open the Jupyter notebook in VS Code
5. Run cells in sequence to reproduce results

---

## Future Improvements

* Hyperparameter tuning for Random Forest
* Trying advanced models like Gradient Boosting
* Handling class imbalance using advanced techniques
* Deploying the model using a web interface

---

## Conclusion

This project demonstrates a complete end to end machine learning pipeline for customer churn prediction. It combines data cleaning, exploratory analysis, model building and interpretation with business focused insights. The final model provides actionable predictions that can help reduce customer churn effectively.

---

## Author

Developed as a hands on machine learning project to demonstrate practical understanding of data driven customer retention strategies.
