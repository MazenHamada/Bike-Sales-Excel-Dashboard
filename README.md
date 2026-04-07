# Bike Sales Excel Dashboard 🚲

## Project Overview
This project focuses on analyzing the demographic data of a retail store's customer base to understand the key characteristics of individuals who purchase bicycles. The goal is to identify trends in income, age, commute distance, and region to help target marketing efforts more effectively.

## Tools Used
* **Microsoft Excel:** Data Cleaning, Pivot Tables, Data Visualization, Dashboard Creation.

## Data Cleaning & Preparation
Before analyzing the data, I ensured the dataset was clean, consistent, and ready for modeling by performing the following steps:
* **Removed Duplicates:** Scanned the dataset and removed duplicate records to prevent skewed aggregations.
* **Handled Missing Values:** Inspected all columns for NULLs or blank cells to ensure data completeness.
* **Standardized Text Variables:** * Converted the `Marital Status` abbreviations from 'M' to 'Married' and 'S' to 'Single'.
  * Converted the `Gender` abbreviations from 'M' to 'Male' and 'F' to 'Female' to improve readability in dashboard labels.
* **Trimmed Whitespace:** Ensured no leading or trailing spaces existed in categorical text columns (like `Occupation` and `Region`) to prevent fragmented groupings in PivotTables.
* **Feature Engineering (Calculated Columns):** Created a new `Age Group` column using nested `IF` formulas to categorize the continuous raw age data into manageable 'Youth', 'Adult', and 'Old' brackets.
* **Custom Sorting Logic:** Reordered the `Commute Distance` variables within the PivotTables to ensure they displayed in logical, sequential order (e.g., ensuring "10+ Miles" appeared at the end of the axis rather than alphabetically at the beginning).
* **Data Type Validation & Formatting:** Verified that all columns were assigned the correct data types and applied uniform currency formatting (with zero decimal places) to the `Income` column for cleaner reporting.
* **Outlier Detection:** Briefly reviewed numerical columns (`Age`, `Income`) using filtering and basic descriptive statistics to ensure there were no logical errors or extreme outliers that would distort the averages.

## Exploratory Data Analysis & Dashboards
Once the data was clean, I utilized Excel Pivot Tables to aggregate the data and find relationships between customer demographics and bike purchases. 

The final interactive dashboard includes slicers for filtering by Region, Marital Status, Education, and Occupation, and highlights the following key metrics:
1. Age vs. Bike Purchase Status
2. Income vs. Bike Purchases by Gender
3. Bike Purchases by Region
4. Commute Distance vs. Bike Purchase Status

## Key Insights
* **The Ideal Customer:** The highest volume of bike buyers are middle-aged adults with a short commute (0-1 miles) and a slightly above-average income.
* **Commute Distance is a Major Factor:** The likelihood of purchasing a bike drops significantly once a customer's commute exceeds 5 miles.
* **Income Correlation:** Across both genders, individuals who purchased a bike had a higher average income than those who did not.
* **Regional Dominance:** North America represents the largest market for bike sales in this dataset, significantly outpacing Europe and the Pacific regions. 

## Files in this Repository
* `Bike_Sales_Dataset.xlsx`: The complete Excel workbook containing the raw data, cleaned data, pivot tables, and the final dashboard.
* `Dashboard.png`: A high-resolution image of the final dashboard.
