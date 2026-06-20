# Data Cleaning & Preprocessing Assignment

## Project Overview
This project demonstrates a complete data cleaning and preprocessing workflow using **Python** and **Pandas**. The provided dataset contains multiple real-world data quality issues that were identified, analyzed, and corrected through a structured cleaning process.

**Dataset:** `dirty_dataset.csv`  
**Size:** 20,300 rows × 15 columns  
**Tools:** Python 3.x, Pandas, NumPy, Matplotlib, Imbalanced-Learn

---

## Objectives

The primary goals of this project are:

- Detect and handle missing values.
- Remove duplicate records.
- Resolve duplicate employee IDs.
- Standardize date formats.
- Convert numeric values stored as strings.
- Fix inconsistent labels and spelling errors.
- Detect and handle outliers.
- Correct invalid values and range violations.
- Clean noisy text data.
- Standardize boolean values.
- Fix data type inconsistencies.
- Address class imbalance.
- Validate and clean dataset schema.

---

## Dataset Issues Solved

### 1. Missing Values
Handled missing values in numeric, categorical, date, boolean, and text columns using appropriate imputation techniques.

### 2. Duplicate Rows
Detected and removed exact duplicate records.

### 3. Duplicate Employee IDs
Identified repeated employee IDs and retained unique records.

### 4. Mixed Date Formats
Converted multiple date formats into a standardized datetime format.

### 5. Numeric Values Stored as Strings
Converted values such as:
- `$91118` → `91118.0`
- `71kg` → `71.0`
- `$219.18` → `219.18`

### 6. Inconsistent Labels
Standardized categorical values such as:
- USA / U.S.A / us / America → United States
- Male / male / M / Man → Male

### 7. Spelling Mistakes
Corrected spelling errors including:
- Dhka → Dhaka
- Chitagong → Chittagong
- Slyhet → Sylhet
- Mrketing → Marketing
- Finace → Finance

### 8. Outlier Treatment
Detected salary outliers using the IQR method and capped extreme values.

### 9. Invalid Values
Fixed:
- Invalid ages (-5, 200, 999)
- Negative prices
- Other unrealistic values

### 10. Noisy Text Cleaning
Removed meaningless review entries such as:
- ok
- bad
- na
- ...
- fine

### 11. Boolean Standardization
Converted mixed boolean representations:
- True
- False
- true
- false
- 1
- 0

into a consistent boolean format.

### 12. Data Type Corrections
Ensured all columns use appropriate data types.

### 13. Range Validation
Validated and corrected values outside acceptable ranges.

### 14. Class Imbalance Handling
Addressed target imbalance using Random Oversampling and documented alternative approaches.

### 15. Schema Validation
Removed useless columns such as completely null columns and verified the final dataset structure.

---

## Project Structure

```text
project-folder/
│
├── README.md
├── data_cleaning.ipynb
├── dirty_dataset.csv
├── cleaned_dataset.csv
└── requirements.txt
```

---

## Technologies Used

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Imbalanced-Learn
- VS Code

---

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
pip install -r requirements.txt
```

---

## Running the Project

1. Open Jupyter Notebook:

```bash
jupyter lab
```

2. Open:

```text
data_cleaning.ipynb
```

3. Run all notebook cells from top to bottom.

4. The cleaned dataset will be generated as:

```text
cleaned_dataset.csv
```

---

## Before vs After Summary

| Issue | Before | After |
|---------|---------|---------|
| Missing Values | Present | Imputed |
| Duplicate Rows | Present | Removed |
| Duplicate IDs | Present | Resolved |
| Date Formats | Mixed | Standardized |
| Numeric Strings | Present | Converted |
| Label Inconsistencies | Present | Standardized |
| Spelling Errors | Present | Corrected |
| Outliers | Present | Treated |
| Invalid Values | Present | Corrected |
| Noisy Reviews | Present | Cleaned |
| Boolean Strings | Mixed | Standardized |
| Wrong Data Types | Present | Corrected |
| Range Violations | Present | Fixed |
| Class Imbalance | Severe | Balanced |
| Schema Issues | Present | Validated |

---

## Requirements

```text
pandas
numpy
matplotlib
imbalanced-learn
```

---

## Deliverables

- Fully documented Jupyter Notebook
- Original dirty dataset
- Cleaned dataset
- README documentation
- Requirements file

---

## Author

Name: Promit Dey

Email (Optional): promit.off19@gmail.com
