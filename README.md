# Retail-Sales-Data-Preparation
This repository contains raw dataset and cleaned dataset using Python libraries.

**RAW Dataset**
The Sales data containing messy sales data from 2021-2025 with 21 columns.

**Cleaned Dataset**
The cleaned Sales dataset using python libraries like Pandas containing only 2024-2025 data with 20 columns.

**Steps to clean data-**
1. Import pandas library to initiate the cleaning.
2. Load the Sales excel sheet(messy data)
3. Perform basic checks like
   Shape- to check the dimension of df
   Head()- to retrieve the top 5 data
   info()- to get the information of df such as column names, column datatypes,  is any column contain null values etc.
   columns- to get the column list of df
4. Check for Nullity using isna() and then drop if there is any null in df.
5. Create a new column 'Month-year' from the order_date column.
6. Customize 'Market' column only into 4 regions(APAC, EMEA, LATAM, NA).
7. Remove extra information from the 'Product_name' column keeping only Product_name info.
8. Filtered the df to only last 2 years i.e 2024-2025 as 'filtered_df' which could improve load time in reporting.
9. Format 'order_id' column as First 2 letters from 'country' in upper + year from 'Month_year' + Last numbers from 'order_id' using slicing. _(Eg- AU-2024-37383)_
10. Drop unnecessary columns from new 'filtered_df' df
11. Save this cleaned df into excel sheet as 'cleaned_sales_data.xlsx'.

## Visualization Project

The cleaned dataset generated in this project was later used to build an interactive Tableau dashboard.

Tableau Dashboard Repository:
https://github.com/Himanshu2311garg/Retail-Analytics-BI-Dashboard
