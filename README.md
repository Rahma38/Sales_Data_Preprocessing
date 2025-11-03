# 🧹 Data Cleaning & Preprocessing

This repository showcases the data cleaning and preprocessing steps applied to a raw dataset to make it ready for analysis. The cleaning process includes handling missing values, removing duplicates, standardizing columns, correcting data types, and treating outliers.

---

## 🔹 Key Steps Performed

### 1️⃣ Handle Missing Values
- Removed NULL or empty values in important columns such as Customer Name.
- Fixed missing or incorrect entries in Ship Date.

### 2️⃣ Remove Duplicates
- Identified and removed duplicate rows to ensure data integrity.

### 3️⃣ Standardize Columns
- Standardized Country names using VLOOKUP.
- Unified Order Date format to dd/mm/yyyy and fixed data types.

### 4️⃣ Correct Ship Dates
- Adjusted Ship Date to be **3 days after Order Date** wherever needed.
- Removed wrong or missing dates.

### 5️⃣ Clean Quantity & Unit PricQuantityty**: Removed negative or unrealistic large valuesUnit Pricece**: UISNUMBER()()** to detect invalid entries and replaced them with medianan**.

### 6️⃣ Handle Outliers in Total
- Calculafive-number summaryry**: Min, Q1, Median, Q3, Max.
- CompuIQRQR** to determlower and upper boundsds**.
- Replaced or treated values outside boundsoutliersrs**.

---

## 📊 Summary by Column

| Column        | Cleaning Steps Applied                                           |
|---------------|-----------------------------------------------------------------|
| Customer Name | Removed null values                                              |
| Country       | Standardized using VLOOKUP                                       |
| Order Date    | Unified format (dd/mm/yyyy) & corrected data type                |
| Ship Date     | Corrected to 3 days after Order Date & removed wrong/missing     |
| Quantity      | Removed negative & unrealistic large values                     |
| Unit Price    | Removed invalid entries & replaced with median                  |
| Total         | Detected outliers using IQR & five-number summary               |
| Entire Data   | Removed duplicates, ensured consistency & readiness for analysis|

---

## 🛠 Tools & Functions UseExcel Functions:s:** ISNUMBER(), VLOOKUP(), MEDIAN()
- **Techniques:** Outlier detection, IQR calculation, data type standardization, duplicate removal

---

✅ The dataset is now cleaned, consistent, and ready for analysis or visualization.
