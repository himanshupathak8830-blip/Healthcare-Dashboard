# Healthcare Dashboard Project

A data-driven healthcare operations dashboard project built from structured Excel datasets and visual dashboard snapshots. This repository appears to be designed for healthcare analytics practice, reporting, and decision-support prototyping using spreadsheet-based data modeling.

---

## Overview

This project organizes core hospital and clinical data domains (patients, doctors, departments, billing, tests, surgeries, inventory, staffing, and rooms) into separate Excel files. The included dashboard images indicate KPI-focused visual reporting for hospital operations.

It is suitable for:
- Healthcare analytics portfolio projects
- Excel/BI dashboard prototyping
- Operational and financial reporting exercises
- Data cleaning and integration practice

---

## Repository Contents

### Data Files (Excel)

| File | Likely Domain |
|---|---|
| `Patient.xlsx` | Patient master or demographic records |
| `Doctor.xlsx` | Doctor/staff provider records |
| `Department.xlsx` | Hospital departments and units |
| `Staff.xlsx` | Operational/non-physician staff details |
| `Rooms.xlsx` | Room allocation/capacity information |
| `Hospital Bills.xlsx` | Billing and payment records |
| `Satisfaction Score.xlsx` | Patient feedback and satisfaction metrics |
| `Medical Tests.xlsx` | Diagnostic test catalog/events |
| `Patient_Tests.xlsx` | Patient-to-test mapping/results |
| `Surgery.xlsx` | Surgery schedules/procedures |
| `Medical Stock.xlsx` | Inventory and stock levels |
| `Supplier.xlsx` | Vendor/supplier details |
| `medicine_patient.xlsx` | Medication dispensation by patient |

### Dashboard Images

The repository also includes several PNG snapshots that likely represent dashboard/report pages:
- `Hospital 1.PNG`
- `hos 2.PNG`
- `hospital 3.PNG`
- `hosptal 4.PNG`
- `hospitl 5.PNG`
- `hospital 6.PNG`

---

## Recommended Data Model

If you plan to rebuild this in Power BI/Tableau/Excel Pivot dashboards, a star-schema-style model can be used:

- **Fact Tables**
  - Billing (`Hospital Bills.xlsx`)
  - Patient Tests (`Patient_Tests.xlsx`)
  - Surgeries (`Surgery.xlsx`)
  - Medication Usage (`medicine_patient.xlsx`)

- **Dimension Tables**
  - Patients (`Patient.xlsx`)
  - Doctors (`Doctor.xlsx`)
  - Departments (`Department.xlsx`)
  - Staff (`Staff.xlsx`)
  - Rooms (`Rooms.xlsx`)
  - Tests (`Medical Tests.xlsx`)
  - Suppliers (`Supplier.xlsx`)

- **Operational Support Tables**
  - Medical stock (`Medical Stock.xlsx`)
  - Satisfaction (`Satisfaction Score.xlsx`)

---

## Example KPI Ideas

This dataset can support dashboards for:

1. **Patient Operations**
   - Total admissions/visits
   - Department-wise patient load
   - Average stay duration (if dates are available)

2. **Clinical Activity**
   - Tests per patient / per department
   - Surgery counts by type and period
   - Doctor utilization metrics

3. **Financial Performance**
   - Total billed amount
   - Average bill per patient
   - Collection efficiency

4. **Inventory & Supply Chain**
   - Low-stock medicine alerts
   - Supplier dependency analysis
   - Inventory turnover proxy metrics

5. **Quality & Experience**
   - Overall satisfaction score trends
   - Department-level patient feedback comparison

---

## How to Use This Repository

1. Open each `.xlsx` file and review column definitions.
2. Standardize key identifiers (e.g., `PatientID`, `DoctorID`, `DepartmentID`) across files.
3. Clean missing/duplicate values and normalize data types.
4. Build relationships in your BI tool.
5. Create KPI visuals and compare with included image snapshots.

---

## Suggested Enhancements

- Add a **data dictionary** for every workbook/sheet
- Include a **single merged dataset** for easier onboarding
- Add **Power BI (`.pbix`)** or **Tableau (`.twb/.twbx`)** source files
- Version large datasets using **Git LFS**
- Add sample SQL scripts for warehouse modeling

---

## Project Status

Active dataset repository for healthcare dashboard analysis and reporting practice.

---

## License

No license file is currently provided. Add a `LICENSE` file if you intend to distribute or reuse this project publicly.
