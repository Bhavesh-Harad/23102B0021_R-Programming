# Lab 1 – Data Cleaning and Missing Value Handling in R

## Project Overview

This repository contains the **R programming implementation for Lab 1**, focusing on exploring, summarizing, and cleaning the **Beijing Multi-Site Air Quality Dataset**.

The main objective of this lab is to programmatically identify incomplete records, handle different types of missing and invalid data, and prepare a clean and reliable dataset for further statistical analysis and modeling.

---

## Objectives

The major objectives of this lab are:

* Import and inspect the air quality dataset.
* Identify different types of missing values.
* Generate a summary of missing values.
* Detect and handle invalid numerical values.
* Perform numerical data imputation using the median.
* Perform categorical data imputation using the mode.
* Implement error handling using `tryCatch()`.
* Verify the dataset after the cleaning process.
* Export the cleaned dataset and analysis results.

---

## Dataset

### Beijing Multi-Site Air Quality Dataset

The dataset contains air quality measurements collected from multiple monitoring stations in Beijing.

Important variables include:

* **PM2.5** – Fine particulate matter
* **PM10** – Particulate matter
* **SO2** – Sulfur dioxide
* **NO2** – Nitrogen dioxide
* **TEMP** – Temperature
* **WSPM** – Wind speed
* **wd** – Wind direction

The original dataset is stored as:

```text
target.csv
```

---

## Key Tasks Implemented

### 1. Data Import and Inspection

The CSV dataset is imported into the R environment and inspected using functions for:

* Dataset structure
* Number of rows and columns
* Initial records
* Variable types

---

### 2. Missing Value Identification

Different types of missing or invalid values are identified, including:

* `NA` – Missing values
* `NULL` – Null objects
* `NaN` – Not-a-Number values
* `Inf` – Positive infinity
* `-Inf` – Negative infinity

---

### 3. Missing Value Summary

A custom R function is used to calculate:

* Total number of missing values
* Percentage of missing values

The results are stored in:

```text
missing_value_summary.csv
```

---

### 4. Invalid Value Handling

Invalid numerical values generated during calculations, such as:

```text
Inf
-Inf
NaN
```

are identified and handled appropriately.

This ensures that invalid observations do not affect further statistical analysis.

---

### 5. Numerical Imputation

Missing values in numerical variables are replaced using their respective **median values**.

Variables include:

```text
PM2.5
PM10
SO2
NO2
TEMP
WSPM
```

Median imputation is used because it is less sensitive to extreme values and is suitable for pollution-related numerical data.

---

### 6. Categorical Imputation

Missing values in categorical variables, such as **wind direction (`wd`)**, are replaced using the **mode**.

The mode represents the most frequently occurring category in the variable.

---

### 7. Error Handling

The R `tryCatch()` function is implemented to handle errors during:

* Variable cleaning
* Data processing
* File operations

This improves the reliability and stability of the R program.

---

### 8. Verification

After the cleaning and imputation process, the dataset is checked again to confirm that missing values have been successfully handled.

Comparative tables and visualizations are generated to compare:

```text
Before Cleaning
        ↓
Missing Value Handling
        ↓
Imputation
        ↓
After Cleaning
```

The final verification confirms that the required missing values have been addressed.

---

## Repository Structure

```text
Lab 1/
│
├── Task1.R
│       └── Main R script containing the data cleaning implementation
│
├── R-Prog-Exp1.ipynb
│       └── Jupyter Notebook containing the R implementation and results
│
├── target.csv
│       └── Original uncleaned dataset
│
├── cleanedTarget.csv
│       └── Final cleaned dataset after imputation
│
├── missing_value_summary.csv
│       └── Summary of missing values before cleaning
│
├── Bar chart of comparison between missing values before and after cleaning.jpg
│       └── Visualization comparing missing values before and after cleaning
│
└── missing_values_comparison.png
        └── Additional missing-value comparison visualization
```

---

## Files Description

| File                                                                           | Description                                                  |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------ |
| `Task1.R`                                                                      | Main R script containing the complete data cleaning process  |
| `R-Prog-Exp1.ipynb`                                                            | Jupyter Notebook containing the R implementation and outputs |
| `target.csv`                                                                   | Original uncleaned air quality dataset                       |
| `cleanedTarget.csv`                                                            | Final dataset after missing-value treatment                  |
| `missing_value_summary.csv`                                                    | Summary of missing-value counts and percentages              |
| `Bar chart of comparison between missing values before and after cleaning.jpg` | Bar chart showing missing values before and after cleaning   |
| `missing_values_comparison.png`                                                | Additional visualization of missing-value comparison         |

---

## Data Cleaning Workflow

The overall workflow followed in this lab is:

```text
Load Dataset
     ↓
Inspect Dataset
     ↓
Check Missing Values
     ↓
Generate Missing Value Summary
     ↓
Identify NA / NULL / NaN
     ↓
Identify Inf / -Inf
     ↓
Handle Invalid Values
     ↓
Numerical Imputation using Median
     ↓
Categorical Imputation using Mode
     ↓
Verify Missing Values
     ↓
Export Cleaned Dataset
```

---

## Technologies Used

* **R**
* **RStudio / Jupyter Notebook**
* **R Kernel**
* **CSV Data**
* **Data Visualization**

### R Concepts Used

* Data frames
* Functions
* Conditional statements
* `NA`, `NULL`, `NaN`
* `is.na()`
* `is.nan()`
* `is.null()`
* `is.infinite()`
* Median calculation
* Mode calculation
* Data filtering
* `tryCatch()`
* CSV import/export
* Data visualization

---

## Results

After applying the complete data-cleaning pipeline:

* Missing numerical values were replaced using median imputation.
* Missing categorical values were replaced using mode imputation.
* Invalid `Inf`, `-Inf`, and `NaN` values were handled.
* A cleaned dataset was successfully generated.
* Missing-value summaries were created.
* Before-and-after visualizations were generated.
* The final dataset was verified after cleaning.

The cleaned dataset is available in:

```text
cleanedTarget.csv
```

---

## Visualizations

The repository contains visualizations comparing the number of missing values before and after the cleaning process.

### Missing Values Comparison

```text
Before Cleaning
       ↓
High/Existing Missing Values
       ↓
Data Cleaning & Imputation
       ↓
After Cleaning
       ↓
Reduced/Handled Missing Values
```

Refer to:

```text
Bar chart of comparison between missing values before and after cleaning.jpg
```

and

```text
missing_values_comparison.png
```

for the generated visual results.

---

## Conclusion

This lab demonstrates a complete **data preprocessing and missing-value handling workflow using R** on the Beijing Multi-Site Air Quality Dataset.

Different types of missing and invalid data were identified and handled using appropriate techniques. Numerical variables were imputed using median values, while categorical variables were imputed using the mode.

The final cleaned dataset provides a more reliable foundation for subsequent **statistical analysis, visualization, and machine learning tasks**.

---

## Author

**Bhavesh Harad**

**Computer Engineering**

**Lab 1 – R Programming / Data Cleaning**

