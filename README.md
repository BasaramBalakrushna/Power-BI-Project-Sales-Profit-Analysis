<!-- README.md for Power BI Project: Sales & Profit Analysis -->

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
**Data Preparation → Cleaning (Power Query) → Modeling → Interactive Reporting**

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

Applied a robust set of transformations to ensure data quality and modeling readiness:

- 🗑️ Remove nulls, errors, duplicates  
- 🔤 Text transforms: uppercase, trim, check length  
- 🔁 Replace values: nulls → 0 or dataset average (as appropriate)  
- 📅 Column formatting: Date/Time, Decimal types  
- ✂️ Split `Date` → Year / Month / Day  
- 📊 Group By → Total Sales per Sales Rep  
- 🔄 Unpivot columns for flexible analysis  
- 📥 Fill Down / Fill Up for missing categorical values  
- 📑 Reorder columns for readability and performance  
- ⚡ Load only final tables to the model for efficiency

---

## 📈 Dashboard Overview

### 🟦 Page 1 — Sales & Profits by Sales Rep
- 📊 Clustered Column Chart: Sales by **Sales Rep & Region**  
- 🥧 Pie Chart: Profit share by **Sales Rep**  
- 📝 Multi-row Card: Total Sales & Profit by Rep  
- 🎛️ Slicers: Year, Month, Day  
- 🔗 Sync Slicers: Linked with Page 2 & Page 3

### 🟩 Page 2 — Sales & Profits by Customer
- 📊 Clustered Column Chart: Sales by **Customer & Region**  
- 🥧 Pie Chart: Profit share by **Customer**  
- 📝 Multi-row Card: Sales, Profit, Rep & Customer details  
- 🎛️ Slicers: Year & Month (example: 2005)

### 🟨 Page 3 — Detailed Table View
- 📋 Table: Year, Month, Day, Sales Rep, Customer, Sales, Profit, Region  
- 🧮 Matrix: Customers (rows) × Sales Reps (columns) → Sales & Profit  
- 🔗 Slicer Sync: Filters applied from Page 1 & Page 2 (invisible filters active)

---

## 🎯 Guided Use Case

**Scenario:** Select **Day = 7** and **Month = January** on Page 1.  
**Result:**  
- ✔ Page 2 displays the matching **customer breakdown**.  
- ✔ Page 3 provides **record-level verification** via Table & Matrix.

---

## ✅ Final Outcome & Business Impact

With clean data and interactive visuals, the dashboard:
- 🔎 Compares Sales Reps & Customers side-by-side  
- 🌍 Highlights Region-wise performance and opportunities  
- 📅 Enables drill-down by Year → Month → Day for trend discovery  
- 📊 Provides cross-validation through Tables & Matrices for auditability

**Business value:** Faster decision-making, clear identification of top-performing reps/customers, and actionable insights to optimize sales and profitability.

---

## 🛠️ Tools & Skills

- **Power BI** — Data modeling, interactive visuals, slicer sync, drill-down  
- **Power Query (M)** — ETL, cleaning, transformation logic  
- **DAX (basic/medium)** — Calculated measures & KPIs (as required)  
- **ETL Concepts** — Append, Merge, Unpivot, Group By, Fill Down/Up  
- **Data Visualization & Storytelling** — Dashboard design for business users

---

## 📁 Repository Structure (Suggested)

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

