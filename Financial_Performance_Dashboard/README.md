# 📊 Financial Performance Dashboard (Power BI)

A fully interactive Power BI dashboard built to help a fictional multi-department company monitor its financial performance. This includes department-wise profitability, cost management, and revenue growth trends over time.

---

## 🚀 Project Objective

Enable the company’s decision-makers to:

- Monitor **total revenue, cost, and profit**
- Track **profit margins** across departments
- Analyze **monthly trends** (MoM/YoY growth)
- Compare **performance across departments**
- (Optional) Visualize **budget vs actuals**

---

## 📁 Data Overview

The project uses a **mock raw financial dataset** with the following columns:

- `Date`
- `Department`
- `Revenue`
- `Cost`
- `Month` (manually created)
- Added:
  - `Dim_Date` (generated using DAX)
  - `Dim_Department` (manually created)

---

## 🔧 Tools & Technologies

| Tool            | Purpose                              |
| --------------- | ------------------------------------ |
| **Power BI**    | Data visualization & modeling        |
| **Power Query** | Data cleaning & transformation       |
| **DAX**         | KPI calculations & time intelligence |
| **GitHub**      | Portfolio & version control          |

---

## 🧹 Data Cleaning (Power Query)

- Removed rows with nulls in key fields
- Fixed data types (e.g., date, text, number)
- Calculated `Profit = Revenue - Cost`
- Trimmed/cleaned text fields
- Removed duplicate rows
- Created manual dimension tables

---

## 🧱 Data Model

> Star Schema:

Dim_Date ─────▶ Fact_Financials ◀───── Dim_Department

All tables connected via primary keys with one-to-many relationships.

---

## 🧮 DAX Measures

| Metric                 | Formula Description                     |
| ---------------------- | --------------------------------------- |
| `Total Revenue`        | SUM of Revenue                          |
| `Total Cost`           | SUM of Cost                             |
| `Total Profit`         | Revenue - Cost                          |
| `Profit Margin %`      | (Profit / Revenue) \* 100               |
| `Revenue MoM Growth %` | % change in Revenue from previous month |
| `Revenue YoY Growth %` | % change in Revenue from previous year  |

---

## 📊 Dashboard Layout

### 1. KPI Section

- Total Revenue, Cost, Profit
- Profit Margin %, MoM/YoY Growth

### 2. Trend Analysis

- Revenue & Profit over time (line charts)

### 3. Department Performance

- Department-wise bar charts for Revenue and Profit Margin
- Matrix table for all KPIs by department

### 4. Slicers

- Date Range
- Department

---

## 📸 Screenshots

| KPI Cards                         | Monthly Trend                           | Department Comparison                    |
| --------------------------------- | --------------------------------------- | ---------------------------------------- |
| ![KPI](screenshots/kpi_cards.png) | ![Trend](screenshots/monthly_trend.png) | ![Dept](screenshots/department_perf.png) |

---

## 🧠 Key Learnings

- Hands-on experience with messy data
- Created dynamic KPIs using DAX
- Practiced best practices in layout & design
- Improved storytelling for finance use cases
- Used dimensional modeling (star schema)

---

---

## 📥 How to Use

1. Download the `.pbix` file
2. Open in Power BI Desktop
3. Refresh the data or plug in your own CSV
4. Explore KPIs, slicers, and visuals

---

## 📌 Credits

> 👤 Created by [Your Name]  
> 📅 Date: June 2025  
> 🏷️ Tags: `Power BI`, `Finance`, `Data Analysis`, `Freelancing`, `DAX`, `Portfolio Project`

---

## 🔗 Let's Connect

- 🌐 [LinkedIn](https://linkedin.com/in/yourprofile)
- 📂 [Portfolio](https://yourportfolio.com)
- ✉️ your.email@example.com

---

## ⭐ If you found this project useful, give it a star!
