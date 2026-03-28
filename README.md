# Income Tax Calculation Sheets — FY 2019-20 to FY 2025-26

Automated Excel workbooks for computing income tax liability of Maharashtra state government employees. Built and maintained by **Kasim Pathan**, Tax Compliance Executive at A A Achkal Services, Solapur.

These sheets are used in real-world practice across **300+ state government offices** handling 100–120 employees each. Data is sourced from **Sevarth Mahakosh** — the Maharashtra Government HRMS portal.

---

## What these workbooks do

Each financial year has its own workbook. The workbook does the following automatically:

1. **Accepts raw payslip data** pasted directly from Sevarth Mahakosh into month-wise worksheets (e.g. `APR-24`, `MAY-24`, ... `MAR-25`)
2. **Reads an employee name list** pasted in the last sheet — and auto-generates one dedicated sheet per employee
3. **Captures head-wise payment figures** (Basic Pay, DA, HRA, allowances, deductions etc.) automatically from the monthly sheets into each employee's sheet
4. **Computes income tax liability** based on applicable slabs for that financial year
5. **Compares Old Tax Regime vs New Tax Regime** and suggests the better option for each employee
6. **Detects salary mismatches** — flags if gross salary or net salary totals do not match, which typically happens when a new pay head is introduced that the sheet has not yet accounted for

---

## Folder structure

```
income-tax-sheets/
│
├── FY 2019-20/
│   └── CALCULATION_SHEET_AUTO_FY_2019-20.xlsb
│
├── FY 2020-21/
│   └── CALCULATION_SHEET_AUTO_FY_2020-21.xlsb
│
├── FY 2021-22/
│   └── CALCULATION_SHEET_AUTO_FY_2021-22.xlsb
│
├── FY 2022-23/
│   └── CALCULATION_SHEET_AUTO_FY_2022-23.xlsb
│
├── FY 2023-24/
│   └── CALCULATION_SHEET_AUTO_FY_2023-24.xlsb
│
├── FY 2024-25/
│   └── CALCULATION_SHEET_AUTO_FY_2024-25.xlsb
│
├── FY 2025-26/
│   └── CALCULATION_SHEET_AUTO_FY_2025-26_100.xlsb
│
└── README.md
```

---

## How to use (step by step)

### Step 1 — Open the workbook for the relevant financial year

Each workbook covers one financial year (April to March).

---

### Step 2 — Paste monthly payslip data

Go to the month-wise worksheets in order:

| Worksheet | Data to paste |
|-----------|--------------|
| `APR-24`  | April 2024 payslip data from Sevarth Mahakosh |
| `MAY-24`  | May 2024 payslip data |
| `JUN-24`  | June 2024 payslip data |
| ...       | Continue for each month |
| `MAR-25`  | March 2025 payslip data |

Copy the payslip table directly from Sevarth Mahakosh and paste it into the respective month's worksheet starting from the designated cell. Do not change the column structure.

---

### Step 3 — Paste employee names

Go to the **last sheet** in the workbook (the Employee Name sheet).

Paste the list of employee names — one name per row — exactly as they appear in the Sevarth Mahakosh payslip data. The workbook will automatically:

- Create one dedicated sheet for each employee
- Pull all head-wise payment figures from each monthly sheet into that employee's sheet

---

### Step 4 — Review the main calculation sheet

The **main calculation sheet** automatically:

- Aggregates the full year's income for each employee
- Computes taxable income after standard deduction and other applicable deductions
- Calculates tax liability under **Old Tax Regime** and **New Tax Regime**
- Highlights which regime results in lower tax for each employee

---

### Step 5 — Check mismatch alerts

If any employee's **gross salary** or **net salary** does not tally across months, the sheet flags a mismatch. This usually happens when:

- A new pay head is introduced in Sevarth Mahakosh mid-year
- An arrear payment is made under a new head not previously mapped
- A deduction head is added or renamed

When a mismatch is flagged, review the new/unrecognised pay head and map it to the correct category in the sheet.

---

## Key features summary

| Feature | Description |
|--------|-------------|
| Month-wise data input | One worksheet per month, paste-ready for Sevarth Mahakosh data |
| Auto employee sheets | One sheet auto-created per employee from the name list |
| Head-wise capture | Automatically maps pay heads to the right income categories |
| Tax computation | Slab-wise calculation as per the relevant Finance Act for that FY |
| Regime comparison | Compares Old vs New Tax Regime and flags the better option |
| Mismatch detection | Alerts when gross or net salary figures don't reconcile |
| Year-wise history | Separate workbook for each FY from 2019-20 to 2025-26 |

---

## Important notes

- All workbooks are in `.xlsb` (Excel Binary Workbook) format for faster performance with large datasets
- Requires **Microsoft Excel** — LibreOffice Calc may not support all formulas and macros
- **All employee data in this repository uses dummy/anonymised figures.** No real PAN numbers, names, or salary details of actual employees are included
- Tax slab rates and standard deduction values are updated each year as per the Union Budget

---

## Financial years covered

| Financial Year | Income Tax Act Version | New Regime Available |
|---------------|----------------------|----------------------|
| FY 2019-20 | Finance Act 2019 | No |
| FY 2020-21 | Finance Act 2020 | Yes (introduced) |
| FY 2021-22 | Finance Act 2021 | Yes |
| FY 2022-23 | Finance Act 2022 | Yes |
| FY 2023-24 | Finance Act 2023 | Yes (New Regime made default) |
| FY 2024-25 | Finance Act 2024 | Yes |
| FY 2025-26 | Finance Act 2025 | Yes |

---

## About the author

**Kasim Pathan**
Tax Compliance & Data Executive — A A Achkal Services, Solapur
M.Com (Advanced Accounting) — Solapur University, 2017

- Email: anispathan20@gmail.com
- LinkedIn: [linkedin.com/in/kasim-pathan](https://linkedin.com/in/kasim-pathan)

These sheets are built from 8 years of hands-on experience handling income tax compliance for Maharashtra state government offices. Feedback and suggestions are welcome.
