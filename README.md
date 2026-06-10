# 📊 HR Analytics Dashboard

A fully interactive **HR Analytics Dashboard** developed using **Microsoft Excel, Power Query, and Power Pivot** to analyze employee workforce data, monitor attrition trends, evaluate salary distribution, and support data-driven HR decision-making through dynamic reporting and visualizations.

---

## 🔥 Project Highlights

* ✔ Cleaned and transformed **2,000+ employee records** using Power Query
* ✔ Performed HR data validation and quality checks
* ✔ Developed interactive KPI dashboards for workforce analysis
* ✔ Built DAX measures using Power Pivot for HR reporting
* ✔ Analyzed employee attrition and workforce trends
* ✔ Created salary distribution and department-wise reports
* ✔ Designed dynamic dashboards using Pivot Charts and Slicers

---

## 🧠 Skills & Tools Used

### 📌 Microsoft Excel

* Advanced Excel
* Pivot Tables
* Pivot Charts
* Conditional Formatting
* Dashboard Development
* Data Validation

### 📌 Power Query

* Data Cleaning
* Remove Duplicates
* Data Transformation
* Handle Null Values
* Standardize Department Names
* TRIM() and Proper Case Formatting

### 📌 Power Pivot

* Data Modeling
* DAX Measures
* KPI Calculations
* Relationship Management

### 📌 HR Analytics

* Workforce Analysis
* Attrition Analysis
* Salary Analysis
* Employee Demographics Reporting
* Hiring Trend Analysis

---

## 🗂 Dashboard Screenshot

<img width="1488" height="703" alt="hr Analytist dashboard" src="https://github.com/user-attachments/assets/2965bc5f-71ab-4fd6-a3e9-2373749f834c" />

---

## 📈 Dashboard Features

### ➤ Workforce Overview

* Total Employees
* Active Employees
* Attrition Rate
* Average Salary

### ➤ Department Analysis

* Employees by Department
* Salary by Department
* Attrition by Department

### ➤ Diversity Analysis

* Gender Distribution
* Location-wise Employee Distribution

### ➤ Recruitment Insights

* Joining Trend by Month
* Hiring Pattern Analysis

### ➤ Interactive Filters

* Department Slicer
* Gender Slicer
* Location Slicer
* Timeline Filter

---

## 📊 DAX Measures Used

### Total Employees

```DAX
Total Employees :=
DISTINCTCOUNT(HR[Employee ID])
```

### Active Employees

```DAX
Active Employees :=
CALCULATE(
    DISTINCTCOUNT(HR[Employee ID]),
    HR[Employment Status] = "Active"
)
```

### Exited Employees

```DAX
Exited Employees :=
CALCULATE(
    DISTINCTCOUNT(HR[Employee ID]),
    HR[Employment Status] = "Exited"
)
```

### Attrition Rate

```DAX
Attrition Rate :=
DIVIDE(
    [Exited Employees],
    [Total Employees]
)
```

### Average Salary

```DAX
Average Salary :=
AVERAGE(HR[Salary])
```

---

## 🧩 Data Cleaning & Transformation Performed

* Removed duplicate Employee IDs
* Standardized department names (HR, hr, Human Resource → HR)
* Handled blank salary values using validation techniques
* Validated Exit Dates against Employment Status
* Removed extra spaces using TRIM()
* Converted text into Proper Case
* Created Month and Year columns from Joining Date
* Performed HR data quality checks

---

## 🗂 Dataset Information

The dataset contains **2,000 employee records** with realistic HR data quality issues to simulate corporate reporting scenarios.

### Dataset Columns

* Employee ID
* Employee Name
* Department
* Designation
* Gender
* Joining Date
* Exit Date
* Salary
* Attendance %
* Location
* Employment Status

### Included Data Challenges

* Duplicate Employee IDs
* Blank Salary Values
* Inconsistent Department Names
* Missing Exit Dates
* Extra Spaces in Text Fields

---

## 📂 Project Files

### 📁 Dashboard File

[Download Dashboard](https://github.com/bhagyashrininawe/HR-Analytics-Dashboard-Excel/blob/main/hr%20report.xlsx)

### 📁 Dataset File

[Download Dataset](https://github.com/bhagyashrininawe/HR-Analytics-Dashboard-Excel/blob/main/HR_Analytics_Messy_Dataset_2000_Rows.csv)

---

## 🎯 Business Value

This dashboard enables HR teams and management to:

* Monitor workforce performance and trends
* Track employee attrition across departments
* Analyze salary distribution patterns
* Understand hiring and recruitment trends
* Support strategic HR decision-making
* Improve workforce planning through data-driven insights

---

## 📌 Key Insights

* Identified departments with higher attrition rates.
* Analyzed salary distribution across departments.
* Monitored monthly employee joining trends.
* Evaluated workforce diversity using gender distribution analysis.
* Delivered actionable HR insights through interactive reporting.

---

## 🚀 Future Enhancements

* Employee Performance Analysis
* Attendance and Leave Management Integration
* Predictive Attrition Analysis using Power BI
* Automated HR Reporting Solutions
