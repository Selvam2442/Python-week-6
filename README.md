# Customer Churn Dataset Generator & Analysis

This project provides a Python-based solution for generating a synthetic customer churn database and performing exploratory data analysis (EDA). It is designed to simulate realistic business scenarios where customer attributes and behaviors influence churn rates.

## Features

- **Synthetic Data Generation**: Uses the `Faker` library to generate realistic names, addresses, and contact information.
- **Realistic Churn Logic**: Implements business rules to simulate churn based on tenure, contract type, and customer support interactions.
- **Data Export**: Automatically saves the generated data into a structured CSV file (`customer_churn_database.csv`).
- **Exploratory Data Analysis (EDA)**:
    - Data cleaning and preprocessing (One-Hot Encoding for categorical variables).
    - Statistical summaries of customer demographics and spending.
    - Visualization of churn distribution and churn rates across different segments like Age and Gender.

## Dataset Overview

The generated dataset contains 1,000 customer records with 14 features:

| Feature | Description |
| :--- | :--- |
| `Customer_ID` | Unique identifier for each customer |
| `Name` | Customer's full name |
| `Age` | Customer age (18-70) |
| `Gender` | Male or Female |
| `City` | Customer's location |
| `Tenure` | Duration of subscription in months |
| `Monthly_Charges` | Recurring monthly bill amount |
| `Total_Charges` | Cumulative charges over tenure |
| `Contract_Type` | Monthly, Yearly, or Two-Year |
| `Internet_Service` | Fiber, DSL, or None |
| `Support_Calls` | Number of customer support interactions |
| `Churn` | Binary indicator (1: Churned, 0: Retained) |

## Churn Simulation Logic
The model uses specific business logic to determine churn: A customer is marked as churned (`1`) if they meet the following criteria:
- **Tenure**: Less than 12 months.
- **Contract Type**: Monthly contract.
- **Support Calls**: More than 3 calls.

## Getting Started

### Prerequisites
Ensure you have Python installed along with the following libraries:
- `pandas`
- `faker`
- `matplotlib`
- `seaborn`

### Installation
```bash
pip install pandas faker matplotlib seaborn
