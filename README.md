# 🧹 Data Cleaning & Preprocessing Report

This repository demonstrates the data cleaning and preprocessing steps applied on a raw dataset to prepare it for analysis. The cleaning process included handling missing values, removing duplicates, standardizing columns, fixing data types, and treating outliers.

---

## 🔹 Key Cleaning Steps

### 1️⃣ Handling Missing Values
- Removed **NULL or empty values** from important columns like Customer Name.
- Cleaned the Ship Date column where some dates were missing or incorrect.

### 2️⃣ Removing Duplicates
- Identified and remoduplicate rowsws** across the dataset.

### 3️⃣ Standardizing Columns
- Standardized the Country column usVLOOKUPUP** to unify country names.
- Unified the Order Date formatdd/mm/yyyyyy** and ensured consistdata typepe**.

### 4️⃣ Correcting Ship Dates
- Fixed Ship Date to be **3 days after Order Date** wherever applicable.
- Removed incorrect or missing dates.

### 5️⃣ Cleaning Quantity & Unit Quantityantity**: Removed negative and unrealistic large vaUnit Price Price*ISNUMBER()MBER()** to detect invalid entries and replaced them wmedianmedian** value.

### 6️⃣ Handling Outliers in Total
- Calculafive-number summaryummary**: Min, Q1, Median, Q3, Max.
- CIQR **IQR** and detlower & upper boundsbounds**.
- Treated values outside booutlierstliers**.

---

## 📊 Cleaning Summary by Column

| Column        | Steps Applied                                                                 |
|---------------|-------------------------------------------------------------------------------|
| Customer Name | Removed null values                                                            |
| Country       | Standardized using VLOOKUP                                                    |
| Order Date    | Unified format (dd/mm/yyyy) & fixed data type                                  |
| Ship Date     | Corrected to 3 days after Order Date & removed wrong/missing entries          |
| Quantity      | Removed negative & unrealistic large values                                   |
| Unit Price    | Removed invalid entries (non-numeric) & replaced with median                  |
| Total         | Outlier detection using IQR & five-number summary                             |
| Entire Data   | Removed duplicates, ensured consistency & readiness for analysis              |

---

## 🛠 Tools & FunctionsExcel Functions:tions:** ISNUMBER(), VLOOKUP(), MEDIAN()
- **Techniques:** Outlier detection, IQR calculation, data type standardization, duplicate removal

---

✅ The dataset is now cleaned and ready for analysis or visualization with consistent, reliable data.
