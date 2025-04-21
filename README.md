# Internship Task Day 1

# Data Cleaning and Preprocessing Task

## **Overview**
This project focuses on cleaning and preprocessing a raw dataset to prepare it for analysis or modeling. The dataset initially contained missing values, duplicate records, inconsistent text formats, and mismatched data types. The steps taken aim to ensure data quality and consistency.

---

## **Steps Taken**

### 1. **Handle Missing Values**
- **Issue**: Columns like `director` and `Cast` contained missing values.
- **Fix**:
  - Removed missing values using `.drop_na()`.

### 2. **Remove Duplicate Records**
- **Issue**: Found `N` duplicate rows.
- **Fix**:
  - Removed duplicates using `.drop_duplicates()`.

### 3. **Standardize Text Data**
- **Issue**: Text inconsistencies in `director` (e.g., NimrÃ³d Antal).
- **Fix**:
  - Converted text to lowercase and standardized values using `.str.lower()` and `.replace()`.

### 4. **Standardize Date Formats**
- **Issue**: Inconsistent date formats in `date` (e.g., "01-01-2022", "2022/01/01").
- **Fix**:
  - Standardized all dates to `dd-mm-yyyy` format using `pd.to_datetime()`.

---

## **Tools and Techniques Used**
- **Tools**:
  - Python (Pandas library).
  - Excel for initial exploration and validation.
- **Techniques**:
  - Mean/Median imputation for missing values.
  - String normalization for text data.
  - `pd.to_datetime()` for date standardization.

---

## **Deliverables**
1. Cleaned dataset: `cleaned_dataset.csv`.
2. Summary of changes (detailed above).

---

## **Key Learnings**
- Importance of data quality in analysis.
- Handling common data issues (missing values, duplicates, formatting).
- Using Pandas for efficient data preprocessing.

---


