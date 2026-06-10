# HR Analytics Dashboard | Excel, Power Query, Power Pivot

## Project Overview

Developed an interactive HR Analytics Dashboard using Microsoft Excel, Power Query, and Power Pivot to analyze employee data and support HR decision-making.

The dashboard provides insights into workforce distribution, attrition trends, salary analysis, gender diversity, and hiring patterns.

---

## Dashboard Preview
[View HR Analytics Dashboard](https://github.com/bhagyashrininawe/HR-Analytics-Dashboard-Excel/blob/main/hr%20Analytist%20dashboard.png?raw=true)

---

## Tools Used

- Microsoft Excel
- Power Query
- Power Pivot
- DAX
- Pivot Tables
- Pivot Charts
- Slicers

---

## Dataset Information

The dataset contains 2,000 employee records with real-world data quality issues for analysis and dashboard development.

### Columns Used

- Employee ID
- Employee Name
- Department
- Designation
- Gender
- Joining Date
- Exit Date
- Salary
- Attendance %
- Location
- Employment Status

---

## Data Cleaning Performed

- Removed duplicate Employee IDs
- Standardized department names
- Handled blank salary values
- Validated exit dates
- Removed extra spaces using TRIM
- Converted text into Proper Case
- Created Month and Year columns
- Performed data quality checks

---

## DAX Measures Created

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
HR[Employment Status]="Active"
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

## Dashboard KPIs

- Total Employees
- Active Employees
- Attrition Rate
- Average Salary

---

## Dashboard Visualizations

- Employees by Department
- Salary by Department
- Gender Distribution
- Attrition by Department
- Joining Trend by Month

---

## Key Insights

- HR department experienced the highest attrition.
- Gender distribution remained balanced.
- Hiring trends varied across months.
- Salary structures differed by departments.

---

## Business Value

This dashboard helps organizations:

- Monitor workforce performance
- Analyze employee attrition
- Support strategic HR decisions
- Track hiring trends
- Improve workforce planning

---
