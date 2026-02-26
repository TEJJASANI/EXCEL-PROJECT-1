Here is a **professional, GitHub-ready README.md** for your Excel project.
It is written like a real data analyst portfolio project and covers **all sheets, formulas, dashboards, KPIs, and business logic**.

You can copy-paste this directly into your repo.

---

# 📊 Excel Analytics Project – Students, Sales & Employees Dashboard

## 🔹 Project Overview

This Excel project demonstrates **end-to-end data analysis using core Excel tools** across three business domains:

* 🎓 Student Performance Analysis
* 💰 Sales Performance Dashboard
* 👨‍💼 Employee Lookup & HR Analytics

The project focuses on **formula-based analytics (no Power Query / no Power BI)** and showcases real analyst skills such as:

* Data cleaning & structuring
* KPI creation
* Conditional logic
* Dynamic lookups
* What-If analysis
* Scenario modelling
* Dashboard-ready metrics

---

# 📁 Dataset Structure

## 1️⃣ Students Sheet – Academic Performance Model

### 📌 Fields

* Student ID
* Name
* Subject Marks (Math, Science, English)
* Enrollment Date
* Total Marks *(calculated)*
* Average Marks *(calculated)*
* Grade *(Nested IF)*
* Topper Flag *(AND logic)*
* Eligibility Flag *(AND logic)*
* Years Since Enrollment *(DATEDIF)*

### 🧮 Key Formulas Used

```excel
Total Marks        = SUM(C2:E2)
Average Marks      = AVERAGE(C2:E2)

Grade              = IF(H2>=80,"A",
                     IF(H2>=60,"B",
                     IF(H2>=40,"C","Fail")))

Topper             = IF(AND(C2>80,D2>80),"Topper","No")

Eligible           = IF(AND(C2>60,D2>60,E2>60),"Yes","No")

Years Since Enroll = DATEDIF(F2,TODAY(),"Y")

Count of Avg > 60  = COUNTIFS(H:H,">60")
```

### 📊 Student KPIs

* Total Students
* Average Score
* % Eligible Students
* Number of Toppers
* Grade Distribution

---

## 2️⃣ Sales Sheet – Regional Sales Analytics

### 📌 Fields

* Sales ID
* Product
* Region
* Salesperson
* Amount
* Date
* Month *(TEXT)*
* Year *(YEAR)*
* Sales Category *(High/Medium/Low)*
* Discount Eligibility

### 🧮 Key Formulas

```excel
Month            = TEXT(F2,"mmm")
Year             = YEAR(F2)

Sales Category   = IF(E2>=30000,"High",
                    IF(E2>=15000,"Medium","Low"))

Discount Flag    = IF(E2>30000,"Yes","No")

Regional Sales   = SUMIF(C:C,"South",E:E)
```

### 📊 Sales KPIs

* Total Revenue
* Revenue by Region
* High-Value Sales Count
* Discount Eligible Sales
* Monthly Sales Trend

---

## 3️⃣ Employees Sheet – Dynamic HR Lookup System

### 📌 Fields

* Employee ID
* Name
* Department
* Salary
* Joining Date

### 🔎 Dynamic Lookup (XLOOKUP Model)

User enters:

* Employee ID
* Required Field (Name / Department / Salary / Joining Date)

Returns value dynamically.

### 📊 HR KPIs

* Total Employees
* Avg Salary
* Employees by Department
* Highest Salary
* Tenure Analysis

---

# 📈 Dashboard Features (Formula-Driven)

## 🎯 KPI Cards

* Total Students / Revenue / Employees
* Avg Marks / Avg Salary
* Eligible Students %
* High Sales %

## 🎛 Interactive Controls

* Slicers (Region, Department, Grade)
* Dynamic lookup input cells
* Scenario Manager for profit simulation

---

# 🔮 What-If Analysis (Profit Simulation)

### Profit Model

```text
Profit = Sales × (1 – Discount) × 0.3
```

### Scenarios

* No Discount
* 10% Discount
* 20% Discount

Used **Scenario Manager** to evaluate impact on total profit.

---

# 🧠 Skills Demonstrated

## ✔ Excel Functions

* SUM, AVERAGE
* IF, Nested IF
* AND
* COUNTIF / COUNTIFS
* SUMIF
* XLOOKUP
* TEXT, YEAR
* DATEDIF

## ✔ Analytical Concepts

* KPI design
* Segmentation (High / Medium / Low)
* Eligibility logic
* Dynamic dashboards
* Scenario modelling
* Business rule implementation

---

# 📊 Business Insights Generated

## 🎓 Students

* Identify toppers using multi-subject criteria
* Track eligibility for scholarships
* Monitor grade distribution
* Analyze student tenure

## 💰 Sales

* Regional performance comparison
* High-value deal tracking
* Discount impact on revenue
* Monthly trend analysis

## 👨‍💼 Employees

* Dynamic HR information retrieval
* Department salary benchmarking
* Tenure and workforce structure

---

# 🚀 How to Use

1. Open the Excel file
2. Use input cells for:

   * Employee ID lookup
   * Scenario selection
3. Apply slicers to filter KPIs
4. Modify discount values to run What-If analysis

* Add **interview explanation section**
* Convert this into a **portfolio-level case study README** 🔥
