# Detecting Outliers in Financial Transactions

## Project Overview

This project focuses on cleaning financial transaction data and identifying unusual transaction patterns using Python. The **Interquartile Range (IQR)** method is used to detect potential outliers in transaction amounts.

The project demonstrates how data cleaning, validation, and outlier detection can support financial risk monitoring and help organizations identify transactions that may require further investigation.

## Business Problem

Financial institutions process a large number of transactions every day. Identifying unusual transactions manually can be difficult and time-consuming.

Traditional rule-based systems often rely on fixed thresholds. These rules may flag legitimate transactions or fail to identify unusual activity that falls below a predefined limit.

This project uses a data-driven approach to identify potential outliers in transaction amounts.

## Project Objectives

- Clean and prepare raw financial transaction data.
- Identify and handle duplicate and missing records.
- Standardize inconsistent data formats and values.
- Validate transaction dates and amounts.
- Detect potential outliers using the IQR method.
- Provide recommendations to support financial risk monitoring.

## Dataset Information

- **Format:** CSV
- **Records:** 4,080 rows (as described for this project)
- **Columns:** 14
- **Dataset versions:** Raw and cleaned

The dataset contains financial transaction information, including fields such as transaction amount, risk score, transaction date, merchant, status, branch, payment method, transaction type, and account type.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- CSV

## Project Workflow

### 1. Data Cleaning and Preprocessing

The following activities were performed:

1. Identified and removed duplicate records.
2. Checked missing values.
3. Replaced blank and whitespace-only cells with missing values.
4. Removed unnecessary leading and trailing spaces.
5. Standardized text formats and letter cases.
6. Converted transaction amounts into numeric format.
7. Converted transaction dates into datetime format.
8. Identified invalid or missing transaction dates.
9. Validated transaction amounts.
10. Checked categorical values and handled missing account types.
11. Performed final data validation.
12. Prepared the cleaned dataset for analysis.

### 2. Outlier Detection Using IQR

The Interquartile Range (IQR) method was used to identify unusual transaction amounts.

**Formula:**

- Q1 = First Quartile (25th percentile)
- Q3 = Third Quartile (75th percentile)
- IQR = Q3 − Q1
- Lower Limit = Q1 − 1.5 × IQR
- Upper Limit = Q3 + 1.5 × IQR

Transactions below the lower limit or above the upper limit were identified as potential outliers.

The identified outliers were stored separately for further analysis rather than automatically removed from the cleaned dataset.

## Business Recommendations

Based on the project approach, financial institutions can:

- Investigate unusual transactions before taking action.
- Prioritize transactions using risk scores and monitoring alerts.
- Apply additional verification when suspicious activity is identified.
- Improve data validation to reduce data-entry and system errors.
- Review legitimate unusual transactions to reduce false alerts.

**Important:** An outlier is not automatically a fraudulent transaction. It is an unusual observation that may require further investigation.

## Expected Outcome

The project demonstrates how Python can be used to clean financial transaction data, validate records, and identify potential outliers. These findings can support better monitoring and informed decision-making.

## Future Scope

- Implement machine learning-based anomaly detection.
- Develop an interactive financial risk monitoring dashboard.
- Explore real-time transaction monitoring.
- Combine transaction patterns with risk scores for improved investigation prioritization.

## Author

**Stenet Sylvia V.**

Aspiring Data Analyst

[GitHub Profile](https://github.com/stenetsylvia-afk)
