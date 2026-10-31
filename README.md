# HR Analytics Dashboard — Employee Attrition Analysis (Excel)

An interactive Excel dashboard that analyzes ~1,470 employee records to find **who leaves the company and why**. Built with Power Query, the Excel Data Model, PivotTables, and slicers.

![Dashboard overview](dash.PNG)

## Business Question

Employee attrition is costly. This project answers:

- What is the overall attrition rate?
- Which job roles, age groups, salary levels, and working conditions are linked to higher attrition?
- Where should HR focus retention efforts first?

## Dataset

- **Records:** ~1,470 employees (one row per employee)
- **Columns:** 38, covering demographics, job details, compensation, satisfaction scores, and tenure
- **Target field:** `Attrition` (Yes / No)
- **Derived fields:** `AgeGroup` and `SalarySlab` for grouping
- A full data dictionary is in the **Metadata** sheet of the workbook.

## Tools

| Area | Tools |
|---|---|
| Data loading and transformation | Excel Power Query |
| Modeling | Excel Data Model |
| Analysis | PivotTables |
| Interactivity | Slicers (Department, Salary Slab) |
| Visuals | Bar, doughnut, and treemap charts, KPI cards |

## Workbook Structure

| Sheet | Purpose |
|---|---|
| `Metadata` | Data dictionary for all 38 columns |
| `Fact Data` | The employee table loaded through Power Query |
| `Working Sheet` | 9 PivotTables that feed the dashboard |
| `Wireframing` | Layout plan for the dashboard |
| `Overview` | The interactive dashboard |

## KPIs

- Total Employees
- Attrition Rate
- Overtime Rate
- Satisfaction Score
- Average Monthly Income

## Key Insights

Figures below are computed on the de-duplicated dataset (1,470 employees, 237 who left).

| Finding | Result |
|---|---|
| Overall attrition rate | **16.1%** |
| Employees working overtime | 28.3% of staff |
| Attrition with overtime vs. without | **30.5% vs. 10.4%** |
| Attrition by salary slab | **21.8%** (up to 5K) vs. **3.8%** (15K+) |
| Highest-attrition job role | **Sales Representative — 39.8%** |
| Attrition by age group | **35.8%** (18–25) vs. 9.2% (36–45) |
| Attrition by marital status | Single **25.5%** vs. Married 12.5% and Divorced 10.1% |
| Attrition by department | Sales 20.6%, HR 19.0%, R&D 13.8% |
| Average monthly income | ~4,787 for those who left vs. ~6,833 for those who stayed |

## Recommendations

Based on the findings, HR could:

1. **Review overtime workload**, since overtime is associated with roughly 3x higher attrition.
2. **Review pay for the lowest salary slab** and for entry-level roles.
3. **Focus retention efforts on Sales Representatives** and on employees aged 18–25.
4. **Track satisfaction and work-life balance** in departments with high attrition.

These are observations from the data, not proof of cause. Attrition has many drivers, and a deeper analysis would be needed to confirm them.

## How to Use

1. Download `HR_Analytics.xlsx` and open it in Excel (Microsoft 365 recommended, since the workbook uses Power Query and the Data Model).
2. Go to the **Overview** sheet.
3. Use the **Department** and **Salary Slab** slicers to filter the KPIs and charts.
4. Click **Data → Refresh All** if you replace the source data.

## Future Improvements

- Complete the **Department** and **Employee** dashboard pages.
- Add a Power BI version of the dashboard.
- Build a simple attrition prediction model in Python.

## Author

**Ahmed Akram Amer** — AI/ML Engineer & Data Analyst

- GitHub: [Ahmed-7-ML](https://github.com/Ahmed-7-ML)
- LinkedIn: [ahmed-akram-kamel-amer](https://linkedin.com/in/ahmed-akram-kamel-amer)
- Portfolio: [ahmed-amer-3ai.vercel.app](https://ahmed-amer-3ai.vercel.app/)
- Email: ahmedakram3ai@gmail.com
