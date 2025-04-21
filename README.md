# Internship Task Day 1

# Data Cleaning and Preprocessing Task

## **Overview**
This project focuses on cleaning and preprocessing a raw dataset to prepare it for analysis or modeling. The dataset initially contained missing values, duplicate records, inconsistent text formats, and mismatched data types. The steps taken aim to ensure data quality and consistency.

---

## **Steps Taken**

### 1. **Handle Missing Values**
- **Issue**: Columns like `Column A` and `Column B` contained missing values.
- **Fix**:
  - Replaced missing numerical values in `Column A` with the column mean.
  - Replaced missing categorical values in `Column B` with "Unknown".
  - Used Pandas functions `.isnull()` and `.fillna()`.

### 2. **Remove Duplicate Records**
- **Issue**: Found `N` duplicate rows.
- **Fix**:
  - Removed duplicates using `.drop_duplicates()`.

### 3. **Standardize Text Data**
- **Issue**: Text inconsistencies in `Column C` (e.g., "USA", "Usa", "us").
- **Fix**:
  - Converted text to lowercase and standardized values using `.str.lower()` and `.replace()`.

### 4. **Standardize Date Formats**
- **Issue**: Inconsistent date formats in `Column D` (e.g., "01-01-2022", "2022/01/01").
- **Fix**:
  - Standardized all dates to `dd-mm-yyyy` format using `pd.to_datetime()`.

### 5. **Validate and Fix Data Types**
- **Issue**:
  - `Column E` (Age) was stored as a string instead of an integer.
  - `Column F` (Dates) was stored as an object instead of a datetime.
- **Fix**:
  - Converted `Column E` to integers and `Column F` to datetime using `.astype()` and `pd.to_datetime()`.

### 6. **Rename Columns**
- **Issue**: Column headers were inconsistent and contained spaces.
- **Fix**:
  - Standardized column names to lowercase and replaced spaces with underscores using `.columns.str.lower().str.replace()`.

### 7. **Outlier Detection and Treatment** (Optional)
- **Issue**: Outliers identified in `Column G` (numerical data).
- **Fix**:
  - Used the Interquartile Range (IQR) method to detect and replace outliers with the column median.

---

## **Tools and Techniques Used**
- **Tools**:
  - Python (Pandas library).
  - Excel for initial exploration and validation.
- **Techniques**:
  - Mean/Median imputation for missing values.
  - String normalization for text data.
  - IQR method for outlier treatment.
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

## **How to Use**
1. Clone this repository.
2. Open the provided script in Python.
3. Run the script to clean your dataset or replicate the steps.
4. Refer to the cleaned dataset (`cleaned_dataset.csv`) for further analysis.

---

Feel free to explore, modify, and expand this project for further learning and improvement!

