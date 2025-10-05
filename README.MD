# Customer Churn Analysis for a Telecom Company

## Project Overview

This project presents an in-depth analysis of customer churn for a fictional telecommunications company. The primary objective is to identify the key factors and patterns that lead to customers discontinuing their services. By leveraging customer demographic data, subscribed services, and contract details, this analysis aims to provide actionable insights that can help the company develop effective retention strategies, reduce churn rates, and improve overall customer satisfaction.

## 🎯 Core Objective

To analyze customer data to uncover patterns and identify the primary drivers behind customer churn. The ultimate goal is to answer the question: **"What are the common characteristics of customers who leave our service?"**

---

## 💾 Dataset Description

The analysis is based on three distinct datasets that provide a holistic view of each customer.

### 1. `customers`

This table contains demographic information about the customers.

| Field          | Description                                           |
|----------------|-------------------------------------------------------|
| `customerID`   | A unique identifier for each customer.                |
| `gender`       | The customer's gender (Male / Female).                |
| `SeniorCitizen`| Indicates if the customer is a senior citizen (1, 0). |
| `Partner`      | Indicates if the customer has a partner (Yes, No).    |
| `Dependents`   | Indicates if the customer has dependents (Yes, No).   |


### 2. `services`

This table details all the services each customer has subscribed to.

| Field            | Description                                                            |
|------------------|------------------------------------------------------------------------|
| `customerID`     | A unique identifier for each customer.                                 |
| `PhoneService`   | Indicates if the customer has a phone service (Yes, No).               |
| `MultipleLines`  | Indicates if the customer has multiple phone lines (Yes, No, No phone service). |
| `InternetService`| The customer's internet service provider (DSL, Fiber optic, No).       |
| `OnlineSecurity` | Indicates if the customer has online security (Yes, No, No internet service). |
| `OnlineBackup`   | Indicates if the customer has online backup (Yes, No, No internet service). |
| `DeviceProtection`| Indicates if the customer has device protection (Yes, No, No internet service). |
| `TechSupport`    | Indicates if the customer has technical support (Yes, No, No internet service). |
| `StreamingTV`    | Indicates if the customer has streaming TV (Yes, No, No internet service). |
| `StreamingMovies`| Indicates if the customer has streaming movies (Yes, No, No internet service). |


### 3. `contracts`

This table includes information about the customer's contract, payment details, and churn status.

| Field           | Description                                                        |
|-----------------|--------------------------------------------------------------------|
| `customerID`    | A unique identifier for each customer.                             |
| `tenure`        | The number of months the customer has been with the company.       |
| `Contract`      | The customer's contract term (Month-to-month, One year, Two year). |
| `PaperlessBilling` | Indicates if the customer uses paperless billing (Yes, No).     |
| `PaymentMethod` | The customer's payment method.                                     |
| `MonthlyCharges`| The amount charged to the customer monthly.                        |
| `TotalCharges`  | The total amount charged to the customer over their tenure.        |
| `Churn`         | Indicates if the customer has left the company (Yes, No).          |

---

## 🛠️ Analysis Approach

The analysis will be conducted following these key steps:

1.  **Data Cleaning and Preprocessing:** Handle missing values, correct data types, and merge the datasets to create a unified view for analysis.
2.  **Exploratory Data Analysis (EDA):** Investigate the relationships between different variables and churn. This will involve:
    * Analyzing the distribution of churned vs. non-churned customers.
    * Visualizing how demographic factors (gender, age, dependents) correlate with churn.
    * Determining which specific services or contract types are associated with higher churn rates.
3.  **Insight Generation:** Synthesize the findings from the EDA to build a profile of a customer who is likely to churn.
4.  **Conclusion and Recommendations:** Provide a summary of the key findings and suggest data-driven strategies to the business for reducing customer churn.