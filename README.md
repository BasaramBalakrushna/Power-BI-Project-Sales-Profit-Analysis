📊 Power BI Project: Sales and Profit Analysis


📂 Data Preparation

We worked with three datasets:


📁 data.csv & additional.csv → Date, Sales Rep, Customer Code, Sales, Profit, Region


📁 customers.csv → Customer Code, Customer Name, Association Date



🔧 Steps Performed:


➕ Appended data + additional → new_data


🔗 Merged new_data with customers using Customer Code


✅ Final table contains: Date, Sales Rep, Customer Code, Sales, Profit, Region, Customer, Association Date



🧹 Data Cleaning & Transformation (Power Query)




Applied the following techniques:


🗑️ Removed nulls, errors, duplicates


🔤 Text filters & transformations (uppercase, trim, length, etc.)


🔁 Replace values (e.g., nulls → 0 or average)


📅 Column formatting (Date/Time, Decimal, etc.)


✂️ Split columns (e.g., Day, Month, Year from Date)


📊 Group By → Total Sales per Rep


🔄 Unpivot columns for analysis


📥 Fill down/up for missing values


📑 Reordered columns for better structure


⚡ Enabled Load only for final tables



📈 Report Pages



Page 1: Sales & Profits by Sales Rep


📊 Clustered Column Chart → Sales by Sales Rep & Region


🥧 Pie Chart → Profit share by Sales Rep


📝 Multi-row Card → Total Sales & Profit by Sales Rep


🎛️ Slicers → Filter by Year, Month, Day


🔗 Sync Slicers → Linked with Page 2 & 3


Page 2: Sales & Profits by Customer


📊 Clustered Column Chart → Sales by Customer & Region


🥧 Pie Chart → Profit share by Customer


📝 Multi-row Card → Sales, Profit, Rep & Customer details


🎛️ Slicer → Year & Month (2005 shown)



📄 Page 3: Detailed Table View



📋 Table → All records (Year, Month, Day, Sales Rep, Customer, Sales, Profit, Region)


🧮 Matrix → Customers (Rows) × Sales Reps (Columns) → Sales & Profit


🔗 Slicer Sync → Linked with Page 1 & 2 (invisible here, but filters apply)



🎯 Use Case Example



👉 Select Day 7 + January on Page 1 →

✔ See corresponding Customer breakdown on Page 2

✔ Verify details in Table & Matrix on Page 3



✅ Final Outcome




With clean data + interactive visuals, we built a Power BI Dashboard that:


🔎 Compares Sales Reps & Customers


🌍 Highlights Region-wise performance


📅 Enables drill-down by Date


📊 Provides cross-validation with Tables & Matrices






✨ This project demonstrates end-to-end Power BI workflow: Data Prep → Cleaning → Modeling → Interactive Reporting.



