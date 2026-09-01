# Lab 2 – Control Flow and Advanced Missing Data Handling in R

## Project Overview

This repository contains the **R programming implementation for Lab 2**, focusing on control flow, data cleaning, missing value handling, loops, vectorized operations, and exception handling.

The lab consists of two main tasks:

1. **Control Flow for Data Cleaning** – Cleaning cardiovascular patient records using the UCI Heart Disease Dataset.
2. **Advanced Missing Data Handling** – Detecting and imputing missing values in the UCI Adult Income Dataset.

---

## Key Tasks Implemented

* **Data Cleaning:** Used `if-else` conditions to detect negative blood pressure values and handle extreme values above 250 mmHg.
* **Exception Handling:** Used `tryCatch()` to handle calculation errors such as division by zero and `NA` values.
* **Performance Comparison:** Compared `for` loops with vectorized operations using `system.time()`.
* **Missing Data Handling:** Detected `NA`, `NULL`, `NaN`, blank strings, and invalid values such as age = 999.
* **Imputation:** Replaced missing numerical values using the median and blank categorical values with `"Unknown"`.
* **Visualization:** Used `naniar` to visualize missing-value patterns.
* **Data Validation:** Used `skimr` to generate summaries of the cleaned datasets.

---

## Datasets

### UCI Heart Disease Dataset

Used for cardiovascular patient data cleaning, outlier handling, and control-flow operations.

### UCI Adult Income Dataset

Used for advanced missing-value detection, cleaning, and imputation.

---

## Repository Structure

```text
Lab 2/
│
├── cleaned_heart_data.csv
│      └── Cleaned Heart Disease dataset
│
├── cleaned_adult_data.csv
│      └── Cleaned Adult Income dataset
│
├── Missing Values barchart.png
│      └── Missing values before and after cleaning
│
├── Missingness pattern after cleaning.png
│      └── Missingness visualization after cleaning
│
├── Task1_summary.png
│      └── Task 1 output summary
│
├── Task2_summary.png
│      └── Task 2 output summary
│
└── R PROGRAMMING LAB PROBLEM STATEMENT.pdf
       └── Lab problem statement and objectives
```

---

## Technologies Used

* **R**
* **RStudio / Jupyter Notebook**
* **naniar**
* **skimr**
* UCI Heart Disease Dataset
* UCI Adult Income Dataset

---

## Workflow

```text
Import Dataset
      ↓
Inspect & Validate Data
      ↓
Detect Missing/Invalid Values
      ↓
Apply Control Flow & Exception Handling
      ↓
Impute Missing Values
      ↓
Compare Loop vs Vectorized Operations
      ↓
Visualize & Validate Results
      ↓
Export Cleaned Dataset
```

---

## Conclusion

This lab demonstrates how **R control-flow statements, loops, vectorized operations, exception handling, and advanced missing-data techniques** can be applied to real-world datasets to produce clean and validated data for further analysis.

---

## Author

**Bhavesh Harad**
Computer Engineering

