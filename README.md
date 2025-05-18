# Employee and Project Management Analytics (Capstone Project - April 2025)

This project is a Python-based analytics solution for improving visibility into employee and project performance. It leverages `pandas` and `numpy` to clean, merge, and analyze datasets, providing management insights and automations to streamline decision-making.

---

## 📌 Project Overview

- **Goal:** Analyze employee and project data to assess costs, track project status, and evaluate performance and seniority.
- **Tools Used:** Python, Pandas, NumPy, Jupyter Notebook
- **Result:** Delivered actionable insights, automated performance evaluations, and implemented business logic to manage designations based on project outcomes.

---

## 📂 Datasets Used

### 1. **Employee Data**
Contains basic employee information.

| ID   | Name            | Gender | City     | Age |
|------|-----------------|--------|----------|-----|
| A001 | John Alter      | M      | Paris    | 25  |
| A002 | Alice Luxumberg | F      | London   | 27  |
| A003 | Tom Sabestine   | M      | Berlin   | 29  |
| A004 | Nina Adgra      | F      | Newyork  | 31  |
| A005 | Amy Johny       | F      | Madrid   | 30  |

### 2. **Seniority Level Data**

| ID   | Designation Level |
|------|-------------------|
| A001 | 2                 |
| A002 | 2                 |
| A003 | 3                 |
| A004 | 2                 |
| A005 | 3                 |

### 3. **Project Data**

| ID   | Project     | Cost     | Status   |
|------|-------------|----------|----------|
| A001 | Project 1   | 1002000  | Finished |
| A002 | Project 2   | 2000000  | Ongoing  |
| A003 | Project 3   | 4500000  | Finished |
| ...  | ...         | ...      | ...      |

*Some project costs are missing and will be imputed during analysis.*

---

## 🔧 Tasks Performed

### ✅ Task 1
Created three separate dataframes and saved them as CSV files:
- `employee.csv`
- `designation.csv`
- `project.csv`

### ✅ Task 2
Handled missing project costs using **running average** (via `for` loop).

### ✅ Task 3
Split full names into:
- `First Name`
- `Last Name`  
Dropped the original `name` column.

### ✅ Task 4
Merged all three dataframes into one final dataframe named `Final`.

### ✅ Task 5
Added a **bonus column**:
- 5% bonus of project cost for employees who completed their projects.

### ✅ Task 6
Demoted employees by 1 designation level for every **Failed** project.
- Removed employees if designation exceeded 4.

### ✅ Task 7
Formatted `First Name`:
- Prefixed "Mr." or "Mrs." based on gender.
- Dropped `gender` column.

### ✅ Task 8
Promoted employees (designation -1) whose **age > 29** using `if` condition.

### ✅ Task 9
Created a new dataframe `TotalProjCost`:
- Columns: `ID`, `First Name`, `Total Project Cost`

### ✅ Task 10
Filtered and displayed employees whose **City name contains the letter 'o'**.

---

## 📈 Skills Demonstrated

- Data cleaning and preparation
- Missing value treatment
- Conditional operations
- Data merging and aggregation
- Looping and logic-based decision making
- Pandas/Numpy function usage
- Business logic implementation

---

## 📁 Files Included

- `employee_data.xls` – Cleaned employee data  
- `designation_level_data.xls` – Seniority data  
- `project_data.xls` – Project cost and status
- `total_project_cost.xls` – Total Project summary
- `pythoncapstone (1).ipynb` – All code with detailed comments and output

---

## 🏁 Outcome

By completing this project, I gained hands-on experience in:

- Solving real-world business problems using Python
- Structuring and automating project workflows
- Applying logical conditions to manage employee designations based on performance
