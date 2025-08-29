# 📊 Power BI Project — **Sales & Profit Analysis**

[![Power BI](https://img.shields.io/badge/Tool-Power%20BI-FFB000?style=for-the-badge&logo=power-bi)]()
[![Data Modeling](https://img.shields.io/badge/Data%20Modeling-ETL-blue?style=for-the-badge)]()
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)]()

---

## ❓ Problem Statement  

The company wanted to **analyze its Sales and Profit performance** by:  
- 📊 **Sales Representative** – Who is generating the highest sales and profit?  
- 🧑‍🤝‍🧑 **Customer** – Which customers contribute the most to revenue and profitability?  
- 🌍 **Region** – How performance varies across different regions  
- 📅 **Time (Year, Month, Day)** – What trends can be observed over time?  

👉 **Goal:** Build an **interactive Power BI dashboard** to provide clear, drill-down insights for better decision-making.

---

## 🚀 Project Summary  

An end-to-end Business Intelligence project demonstrating how raw, fragmented sales data is transformed into an actionable Power BI solution.  

**Workflow:**  
`Data Preparation → Cleaning (Power Query) → Modeling → Interactive Reporting`

---

## 📂 Data Sources  

We worked with **3 datasets**:  

- 📁 `data.csv` & `additional.csv`  
  *Columns:* `Date, Sales Rep, Customer Code, Sales, Profit, Region`  
- 📁 `customers.csv`  
  *Columns:* `Customer Code, Customer Name, Association Date`  

**Modeling steps:**  
- ➕ Append `data.csv` + `additional.csv` → `new_data`  
- 🔗 Merge `new_data` with `customers.csv` on **Customer Code**  
- ✅ Final table: `Date, Sales Rep, Customer Code, Sales, Profit, Region, Customer Name, Association Date`

---

## 🧹 Data Cleaning & Transformation (Power Query)  

- 🗑️ Removed nulls, errors, duplicates  
- 🔤 Standardized text (uppercase, trim, etc.)  
- 🔁 Replaced values (nulls → 0 or averages as needed)  
- 📅 Split `Date` into **Year, Month, Day**  
- 📊 Aggregated **Sales by Sales Rep**  
- 🔄 Unpivoted columns for flexible analysis  
- 📥 Used **Fill Down/Fill Up** to handle missing categories  
- ⚡ Optimized by loading only clean final tables into model  

---

## 📈 Dashboard Overview  

### 🟦 Page 1 — Sales & Profits by Sales Rep  


<img width="1123" height="625" alt="Sales_Rep" src="https://github.com/user-attachments/assets/0f98fece-5bce-4708-b04f-01761158823d" />



- 📊 **Clustered Column Chart**: Sales by Sales Rep across regions (East, North, South, West)  
- 🥧 **Pie Chart**: Profit distribution by Sales Rep  
- 📝 **Cards**: Total Sales & Profit by each Rep  
- 🎛️ **Slicers**: Year, Month, Day for drill-down  
- 🔗 **Sync**: Connected with Page 2 & 3  

📌 **Insight**: Bruce, Abhay, and Charley are top performers, while others show varied contributions across regions.  

---

### 🟩 Page 2 — Sales & Profits by Customer  

<img width="1125" height="628" alt="Customer" src="https://github.com/user-attachments/assets/66f48cf5-0e64-4044-be39-60cdf3597fc0" />



- 📊 **Clustered Column Chart**: Sales by Customers across regions  
- 🥧 **Pie Chart**: Profit contribution by Customers  
- 📝 **Cards**: Top customers with linked Sales Reps  
- 🎛️ **Slicers**: Year & Month for filtering  

📌 **Insight**: Shah Associates and Namint Enterprises generate the highest revenue, while other customers bring moderate profitability.  

---

### 🟨 Page 3 — Detailed Table View  

<img width="1122" height="632" alt="Tables" src="https://github.com/user-attachments/assets/ccf7c393-2623-44f1-81c2-ca78ff25acf6" />



- 📋 **Table View**: Record-level data (Year, Month, Day, Rep, Customer, Sales, Profit, Region)  
- 🧮 **Matrix View**: Customers × Sales Reps → Sales & Profit breakdown  
- 🔗 Slicer Sync ensures filters apply consistently across pages  

📌 **Insight**: Provides transparency and validation for numbers shown in Page 1 & 2 dashboards.  

---

## 🎯 Use Case Example  

👉 Select **Day = 7** and **Month = January** on Page 1.  

✔ Page 2 updates with **customer breakdown**  
✔ Page 3 shows **row-level records** for validation  

---

## ✅ Final Outcome & Business Impact  

With clean data and interactive visuals, the dashboard:  
- 🔎 Identifies **top-performing Sales Reps & Customers**  
- 🌍 Highlights **region-wise opportunities**  
- 📅 Enables **time-based trend analysis**  
- 📊 Offers **audit-friendly views** for cross-checking  

**Business Value:** Faster decisions, clear insights, and ability to focus on **high-profit customers & reps**.  

---

## 🛠️ Tools & Skills  

- **Power BI** – data modeling, visuals, slicer sync  
- **Power Query (M)** – ETL & transformations  
- **DAX** – custom measures  
- **Data Visualization & Storytelling** – professional dashboarding  

---

## 📁 Repository Structure  

/PowerBI-Sales-Profit-Analysis
│
├─ data/
│ ├─ data.csv
│ ├─ additional.csv
│ └─ customers.csv
│
├─ reports/
│ └─ PowerBI_Report.pbix
│
├─ docs/
│ ├─ data_dictionary.md
│ └─ transformation_steps.md
│
└─ README.md
