# 🧹 Data Cleaning & Preprocessing

This repository shows the data cleaning steps applied on a raw dataset to make it ready for analysis. The cleaning process includes handling missing values, removing duplicates, standardizing columns, correcting data types, and treating outliers.

---

## Key Steps

### 1. Handle Missing Values
- Removed NULL or empty values from critical columns like Customer Name.
- Fixed missing or incorrect entries in Ship Date.

### 2. Remove Duplicates
- Identified and removed duplicate rows across the dataset.

### 3. Standardize Columns
- Standardized Country names using VLOOKUP.
- Unified Order Date format to dd/mm/yyyy and ensured correct data type.

### 4. Correct Ship Dates
- Adjusted Ship Date to be 3 days after Order Date.
- Removed wrong or missing dates.

### 5. Clean Quantity & Unit Price
- Quantity: Removed negative values and unrealistic large values.
- Unit Price: Used ISNUMBER() to detect invalid entries and replaced them with the median.

### 6. Handle Outliers in Total
- Calculated the five-number summary: Min, Q1, Median, Q3, Max.
- Computed IQR and determined lower and upper bounds.
- Treated values outside bounds as outliers.

---

## Summary by Column

| Column        | Cleaning Steps Applied                                   |
|---------------|---------------------------------------------------------|
| Customer Name | Removed null values                                     |
| Country       | Standardized using VLOOKUP                               |
| Order Date    | Unified format (dd/mm/yyyy) & fixed data type         |
| Ship Date     | Corrected to 3 days after Order Date & removed wrong/missing |
| Quantity      | Removed negative & unrealistic large values            |
| Unit Price    | Removed invalid entries & replaced with median         |
| Total         | Outlier detection using IQR & five-number summary      |
| Entire Data   | Removed duplicates & ensured data consistency          |

---

## Tools & Functions Used
- Excel Functions: ISNUMBER(), VLOOKUP(), MEDIAN()
- Techniques: Outlier detection, IQR calculation, data type standardization, duplicate removal

---

✅ The dataset is now clean, consistent, and ready for analysis or visualization.
