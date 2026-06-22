# Customer Churn Dataset Generator & Analysis

**Created by: Maria Antony Selvam S**

This project is a Python-based synthetic data generation and analysis system for customer churn prediction. It creates a realistic customer churn dataset using the Faker library and performs Exploratory Data Analysis (EDA) to understand customer behavior, spending patterns, and churn trends.

The project is useful for learning data analysis, machine learning preprocessing, and business decision-making using customer data.

---

## Project Screenshots

### Dataset Preview
![Dataset Preview](screenshots/dataset-preview.png)

### Churn Distribution Chart
![Churn Distribution](screenshots/churn-distribution.png)

### Churn by Gender
![Churn by Gender](screenshots/churn-by-gender.png)

### Churn by Age Group
![Churn by Age Group](screenshots/churn-by-age-group.png)

---

## Features

- Generates 1,000 synthetic customer records
- Uses Faker to create realistic customer names, cities, and details
- Applies business-based churn simulation logic
- Saves the dataset as a CSV file
- Performs data cleaning and preprocessing
- Uses One-Hot Encoding for categorical columns
- Provides statistical summaries
- Visualizes churn distribution and customer segments
- Helps understand how tenure, contract type, and support calls affect churn

---

## Dataset Overview

The generated dataset contains customer information with important business-related features.

| Feature | Description |
| :--- | :--- |
| Customer_ID | Unique ID for each customer |
| Name | Customer full name |
| Age | Customer age between 18 and 70 |
| Gender | Male or Female |
| City | Customer location |
| Tenure | Subscription duration in months |
| Monthly_Charges | Monthly bill amount |
| Total_Charges | Total amount paid by the customer |
| Contract_Type | Monthly, Yearly, or Two-Year contract |
| Internet_Service | Fiber, DSL, or None |
| Support_Calls | Number of support calls made |
| Churn | 1 means churned, 0 means retained |

---

## Churn Simulation Logic

A customer is marked as churned when the following conditions are met:

- Tenure is less than 12 months
- Contract type is Monthly
- Support calls are more than 3

This logic simulates a realistic business scenario where new customers with monthly plans and frequent support issues are more likely to leave the service.

---

## Technologies Used

- Python
- Pandas
- Faker
- Matplotlib
- Seaborn
- CSV
  <img width="1276" height="821" alt="image" src="https://github.com/user-attachments/assets/f5c45d2c-e745-4c4b-94e5-96e5a1c2438d" />


---

## Installation

Install the required Python libraries:

```bash
pip install pandas faker matplotlib seaborn
