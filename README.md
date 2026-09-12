# HR Analytics Dashboard | Power BI

An interactive HR analytics dashboard built in Power BI to give HR teams a clear view of workforce composition, promotion readiness, retrenchment planning, satisfaction, overtime, and role-level trends.

**[Open the interactive Power BI report](https://app.powerbi.com/reportEmbed?reportId=76433a27-ff42-4edc-b69a-6bbb9d68f003&autoAuth=true&ctid=f4669cc9-6065-4d34-9017-684988b21f7a)**

## Demo video

https://github.com/user-attachments/assets/42ba1cdd-680e-45d5-a861-e4ec0dfd6316

[Download the local demo video](<HR Dashboard Video demo.mp4>)

## Dashboard highlights

| Metric | Result |
| --- | ---: |
| Total employees | 1,470 |
| Male employees | 882 (60%) |
| Female employees | 588 (40%) |
| Due for promotion | 72 (4.90%) |
| Not due for promotion | 1,398 (95.10%) |
| Due for retrenchment | 117 (8.0%) |
| Active workforce | 1,353 (92.0%) |

## Key insights

- The workforce is male-majority (60%), with women representing 40% of employees.
- Only 72 employees are due for promotion, enabling targeted succession and development conversations rather than broad interventions.
- 117 employees are flagged for retrenchment review; this is the most immediate workforce-planning action area.
- Research & Development carries the largest flagged population: **47** people due for promotion and **74** due for retrenchment. Sales follows with **23** and **36**, respectively; Human Resources has **7** retrenchment flags.
- Sales Executive is the largest job role (326 employees), followed by Research Scientist (292) and Laboratory Technician (259), making these roles important for staffing and retention planning.
- Job satisfaction is weighted toward the high category (569 employees), ahead of low (459) and medium (442). The dashboard also surfaces overtime and distance-from-office patterns for further investigation.

## Report pages

### Home - workforce overview

The landing page presents the headline employee, gender, promotion, retrenchment, active-worker, service-years, job-level, and commuting-distance metrics.

![Home dashboard](<Screenshot 2026-08-01 104413.png>)

### Action - people requiring attention

This page provides employee-level lists for retrenchment and promotion actions, making the flagged groups easy to review and follow up.

![Action dashboard](<Screenshot 2026-08-01 104431.png>)

### Detail - departmental and role analysis

The detail page compares promotion and retrenchment requirements by department, alongside job satisfaction, overtime, ratings, and job-role totals.

![Detail dashboard](<Screenshot 2026-08-01 104453.png>)

## What was built

- **Data cleaning and transformation:** prepared the HR source data and supporting promotion/retrenchment tables for analysis.
- **Data modelling:** connected employee attributes with employee-name, promotion, and retrenchment data to support cross-page reporting.
- **DAX measures:** created measures for total employees, gender split, promotion status, active workers, retrenchment status, satisfaction, and other KPI calculations.
- **Blank and error handling:** applied logic to keep KPI cards and visuals reliable when data is missing or invalid.
- **Dynamic navigation:** used page-navigation controls to move between Home, Action, and Detail views.

## Project files

| File | Purpose |
| --- | --- |
| [Power BI HR Dashboard.pbix](<Power BI HR Dashboard.pbix>) | Editable Power BI report |
| [HR Analytics Data.csv](<HR Analytics Data.csv>) | Main HR dataset |
| [HR employee data.csv](<HR employee data.csv>) | Employee-name lookup data |
| [promotion.csv](promotion.csv) | Promotion-status input |
| [trench.csv](trench.csv) | Retrenchment-status input |
| [HR Dashboard Video demo.mp4](<HR Dashboard Video demo.mp4>) | Dashboard walkthrough |

## Embed on a website

Use the following HTML where embedded Power BI content is supported:

```html
<iframe
  title="HRDB"
  width="1140"
  height="541.25"
  src="https://app.powerbi.com/reportEmbed?reportId=76433a27-ff42-4edc-b69a-6bbb9d68f003&autoAuth=true&ctid=f4669cc9-6065-4d34-9017-684988b21f7a"
  frameborder="0"
  allowfullscreen="true">
</iframe>
```

> The embed can only load for viewers who have the required Power BI access and authentication.
