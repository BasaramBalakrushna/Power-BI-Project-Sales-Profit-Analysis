# Power BI Project Summary: Sales and Profit Analysis by Sales Rep and Customers

1. Data Preparation
We worked with three datasets:

data.csv and additional.csv: Contain Date, Sales Rep, Customer Code, Sales, Profit, Region

customers.csv: Contains Customer Code, Customer Name, Association Date

 Steps Performed:
Appended data and additional into one table → named it new_data

Merged new_data with customers using the Customer Code as the key
→ Now the new_data table contains all the columns:
Date, Sales Rep, Customer Code, Sales, Profit, Region, Customer, Association Date

2. Data Cleaning & Transformation (Power Query)
We applied the following techniques to clean and shape the data:

 Removed nulls, errors, and duplicates

 Text filters (equals, begins with, etc.)

 Replace values (e.g., replacing nulls with 0 or average)

 Formatted columns (Date/Time, Decimal, etc.)

 Text transformations (uppercase, lowercase, trim, length)

 Split columns (e.g., split full name or date into day, month, year)

 Group by to summarize (e.g., total sales per rep)

 Unpivot columns for better analysis structure

 Fill down/up for handling missing values

 Moved columns for better data structure

 Enable Load only for final tables used in visuals

 3. Report Pages Overview
 Page 1: Sales & Profits by Sales Rep
 Clustered Column Chart: Sales by Sales Rep and Region

 Pie Chart: Profit share by Sales Rep

 Multi-row Card: Shows total Sales and Profit by Sales Rep

 Slicers: Filter by Year, Month, and Day

 Sync Slicers: Year, Month, Day are synced with Page 2 & 3 but visible only on Page 1

 Page 2: Sales & Profits by Customer
 Clustered Column Chart: Sales by Customer and Region

 Pie Chart: Profit share by Customer

 Multi-row Card: Sales, Profit, Sales Rep, and Customer details

 Slicer: Filter by Year and Month (only 2005 shown)

 Page 3: Detailed Table View
 Table: Shows all records with Year, Month, Day, Sales Rep, Customer, Sales, Profit, Region

 Matrix: Cross-validation – Rows as Customers, Columns as Sales Reps, Values as Sales and Profit

 Slicer Sync: Linked with Page 1 & 2 (invisible on this page but filters apply)

 Use Case: Select "Day 7", "January" on Page 1 → Check corresponding detailed data in Page 2 & 3

  Final Outcome
With clean and connected data, and interactive slicers across pages, we created a powerful and user-friendly sales dashboard that:

Compares Sales Reps and Customers

Highlights Region-wise performance

Allows drill-down by date

Enables data verification through tables and matrices.



