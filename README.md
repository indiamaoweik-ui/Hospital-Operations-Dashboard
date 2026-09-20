# MediTrack Data Dashboard

## Project Overview

Developed a Power BI dashboard using 15,001 hospital records from MediTrack Health UK to analyze financial performance, patient activity, procedure wait times, and hospital resource utilization.

The goal was to use healthcare operations data to identify important trends, evaluate performance, and uncover opportunities for improving hospital efficiency.

## Business Questions

The dashboard was designed to answer five key business questions:

1. **How has revenue changed month-to-month and year-to-year?**
2. **Which medical specialty contributes the highest share of total revenue?**
3. **Which visit types drive revenue?**
4. **Which procedures have the longest average wait times?**
5. **Are visit volumes increasing faster than staffing and resources?**

## Data & Tools

- **Data:** MediTrack Health UK
- **Records:** 15,001
- **Tool:** Microsoft Power BI
- **Data Preparation:** Power Query
- **Data Modeling:** Star Schema
- **Analysis:** DAX
- **Measures Created:** 18

## Analytical Process

I first cleaned and transformed the hospital data using Power Query and organized it into a star-schema data model consisting of one fact table and eight dimension tables.

I then created 18 DAX measures to analyze financial performance, patient activity, procedure wait times, and resource utilization.

The analysis examined revenue trends over time, differences in revenue contribution across medical specialties and visit types, procedure-level wait times, and the relationship between patient volume and available staffing and resources.

While analyzing procedure wait times, I recognized that average wait time alone might not provide the complete picture because unusually long waits can disproportionately affect the mean. I therefore added median wait time as a second measure and compared the results across procedure categories.

This additional analysis provided more context for interpreting the wait-time data and helped inform the project's operational recommendation.

## Key Insights

- The dashboard identified differences in revenue performance across months, years, medical specialties, and visit types.
- The analysis highlighted procedure-level differences in average wait times, allowing potential operational bottlenecks to be identified.
- Median wait times were identical across minor, diagnostic, and surgical procedures, providing additional context when comparing the procedure categories.
- The wait-time analysis identified surgical procedures as an area where additional staffing could potentially improve patient flow.
- Based on the analysis, the project recommended evaluating a reallocation of approximately **10% of staff toward surgical procedures**, with a projected **15% reduction in surgical wait times**.

## Dashboard

The Power BI dashboard provides an interactive view of hospital financial and operational performance, allowing users to explore revenue trends, medical specialties, visit types, patient volumes, staffing/resources, and procedure wait times.

## Files

- `MediTrack_Data_Dashboard.pdf` — PDF version of the Power BI report
- `MediTrack_Data.pbix` — Original Power BI project file
- `MediTrack_Data_Model.png` — Visual representation of the Power BI data model

## Conclusion

This project demonstrates how I used Power BI to move from raw healthcare data to business-focused insights and an operational recommendation.

Rather than analyzing a single metric, I examined multiple dimensions of hospital performance, including revenue, patient activity, procedure wait times, and resource utilization. The wait-time analysis also demonstrated the importance of questioning whether a single metric tells the complete story, leading me to compare mean and median wait times before developing the staffing recommendation.
