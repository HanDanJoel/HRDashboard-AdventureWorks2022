# HRDashboard-AdventureWorks2022
# HR Analytics Dashboard – AdventureWorks Data

## Project Overview

This interactive Power BI dashboard provides key HR insights using data from the AdventureWorks2022 database. It allows users to explore employee demographics, hiring trends, department headcounts, and compensation details through a clean and dynamic interface.

The dashboard is designed to demonstrate not only visualization skills in Power BI, but also backend data preparation using SQL.

---

## Key Features

- **KPI Cards**:
  - Total Employees
  - Average Tenure
  - Average Salary
  - % Female Employees
  - Average Age

- **Charts and Visuals**:
  - Employees Hired by Year (Line Chart)
  - Headcount by Department (Bar Chart)
  - Gender Distribution (Donut Chart)
  - Employees by Department and Age Group (Stacked Bar Chart)

- **Dynamic Slicers** (using bookmarks):
  - Users can toggle between filtering by `Tenure`, `Shift`, or `StateProvince` using custom buttons.
  - Each filter appears one at a time in the same space to save layout real estate.

---

## Tools & Technologies

- **Power BI Desktop**
- **SQL Server Management Studio (SSMS)**
- **AdventureWorks2022 Sample Database**
- DAX (Data Analysis Expressions) for calculated columns and measures
- SQL Views for efficient data prep

---

## How It Works

### SQL View

A view named `vw_HRDashboard` was created to combine key employee data from multiple tables in the AdventureWorks2022 database. The view includes:
- Employee ID and Name
- Gender
- Job Title
- Department
- Hire Date
- Tenure (in years)
- Salary
- Location (StateProvince)
- Shift
- Birth Date

### Power BI Import

The view was imported into Power BI, and additional DAX calculations were created:
- `Age` (based on birth date)
- `Tenure Bucket` and `Age Group` (to group values for visual clarity)
- Measures for totals and averages

### Bookmarks & Buttons

The dashboard includes dynamic slicers that are shown/hidden using bookmarks and buttons. Users can switch between filters (`Tenure`, `Shift`, or `State`) without cluttering the interface.

---

## Interactivity & UX

- All visuals respond to selected filters
- Clean layout using a dark theme with blue accents
- Slicers and KPIs aligned for maximum readability

---

## Files Included

- `HRDashboard.pbix`: Power BI file with full report and visuals
- `README.md`: This file
- `vw_HRDashboard.sql`: SQL script used to create the view

---


## Note

This dashboard uses sample data only (AdventureWorks2022) and is intended for demonstration purposes.
