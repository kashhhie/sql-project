# Human Resources Data - README

## Overview
This dataset contains employee records for a human resources management system. The data includes comprehensive information about employee demographics, employment history, and organizational placement.

## File Details
- **Filename:** `Human Resources.csv`
- **Format:** Comma-separated values (CSV)
- **Total Records:** 22,215 employee records
- **Encoding:** UTF-8

## Data Dictionary

| Column | Data Type | Description |
|--------|-----------|-------------|
| `id` | String | Unique employee identifier (e.g., 00-0037846) |
| `first_name` | String | Employee's first name |
| `last_name` | String | Employee's last name |
| `birthdate` | Date | Date of birth (Mixed format: MM-DD-YY or M/D/YYYY) |
| `gender` | String | Gender (Male, Female) |
| `race` | String | Race/Ethnicity classification (e.g., White, Asian, Hispanic or Latino, Black or African American, Two or More Races, American Indian or Alaska Native) |
| `department` | String | Department name (e.g., Engineering, Sales, Business Development, Services, Product Management, Accounting, Legal) |
| `jobtitle` | String | Job title/position held |
| `location` | String | Work location type (Headquarters, Remote) |
| `hire_date` | Date | Employment start date (Mixed format: MM-DD-YY or M/D/YYYY) |
| `termdate` | DateTime | Employment termination date/timestamp (Empty if currently employed) |
| `location_city` | String | City of work location |
| `location_state` | String | State of work location |

## Data Characteristics
- **Active vs. Terminated:** The `termdate` column is empty for active employees and contains a datetime value for terminated employees
- **Date Format Inconsistency:** Dates use mixed formats (MM-DD-YY and M/D/YYYY) - data cleaning may be needed
- **Location Data:** Employees are located primarily in Cleveland, Ohio and Flint, Michigan
- **Departments:** Multiple departments represented including Engineering, Sales, Business Development, Services, Product Management, Accounting, and Legal

## Notes
- Some employee IDs follow the format XX-XXXXXXX
- All location data appears to be mapped to either Headquarters or Remote work arrangements
- The dataset includes both currently employed and terminated employees
- Race/Ethnicity categories cover standard EEOC classifications
