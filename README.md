# E-Commerce Data Cleaning and Preparation Project

## 📌 Project Overview
This project was completed as part of my Data Analytics Internship at **Decode Labs**. The main goal was to clean, format, and prepare a raw e-commerce dataset containing 1,200 sales records using Python and Pandas.

## 🛠️ Key Actions Taken
1. **Data Profiling:** Loaded the raw dataset and inspected the shape, columns, and initial rows to understand the structure.
2. **Handling Missing Values:** Identified 309 null values in the `CouponCode` column and replaced them with 'NO_COUPON'. Verified that no other columns had missing data.
3. **Duplicate Management:** Implemented logical checks for both complete row duplicates and unique `OrderID` duplicates to ensure data integrity (0 duplicates were found).
4. **Data Formatting & Type Casting:** 
   - Converted the `Date` column to standard datetime format.
   - Casted numerical columns (`Quantity`, `ItemsInCart`) to integers and price columns (`UnitPrice`, `TotalPrice`) to floats.
   - Stripped all leading/trailing white spaces and converted string columns (`Product`, `PaymentMethod`, `OrderStatus`, `ReferralSource`) to UPPERCASE.
5. **Data Export:** Exported the finalized, clean dataset into a new file named `Final_Cleaned_Ecom_Data.csv`.

## 📂 Repository Contents (Inside PROJECTS 1 Folder)
* `store_data.xlsx` - Raw uncleaned e-commerce dataset.
* `Cleaned_Data_Python.ipynb` - Jupyter Notebook containing the clean Python code and markdown step explanations.
* `Final_Cleaned_Ecom_Data.csv` - The final production-ready cleaned data file.

## 📊 Project Visuals and Outputs

### 1. Missing Data Profiling
Below is the snapshot of the missing value inspection showing 309 missing values in the CouponCode column:
![Missing Value Profile](PROJECTS 1/missing_value_count.png)

### 2. Duplicate Integrity Check
Output showing that no duplicate rows or duplicate OrderIDs were present in the dataset:
![Duplicate Check](PROJECTS 1/duplicate_check.png)

### 3. Data Formatting (Date & Text)
Output verifying the successful correction of date strings and uppercase text conversion:
![Data Formatting](PROJECTS 1/Correct_date_format.png)

### 4. Final Verification Summary
Final data types and shape profiling before successfully exporting the cleaned file:
![Final Summary](PROJECTS 1/Final_summary.png)
