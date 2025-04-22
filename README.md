Employee Attrition Analysis and Projection Dashboard

Project Overview
The objective of this project was to analyze employee attrition patterns within an organization and project future attrition risk using Power BI. By identifying the key drivers of attrition—such as job satisfaction, income level, and department differences—HR decision-makers can proactively target high-risk employee segments and improve retention strategies.

Steps Taken

Dataset Preparation
The dataset used was based on realistic HR data, including employee demographics, department, satisfaction ratings, tenure, job role, and attrition status. Key features included Department, Monthly Income, Years at Company, Job Satisfaction, Attrition, Environment Satisfaction, and Employee Number.

Data Modeling and Calculations

Calculated Columns
An Adjusted Job Satisfaction column was created to standardize satisfaction levels and enable more intuitive visual mapping.
A Tenure Bucket column was created to group employees into tenure ranges such as 0-1 years, 2-3 years, 4-5 years, 6-10 years, 11-20 years, and 20+ years.

Measures using DAX
The Attrition Rate was calculated as the number of employees who left divided by the total number of employees.
A Projected Attrition Rate was calculated based on average job satisfaction. A base attrition rate of 25 percent was used, and for every point increase in satisfaction, the attrition rate was reduced by 5 percent. This provided a simulated projection showing how increased satisfaction could reduce future attrition. Minimum value was capped at zero.

Slicers Used
To enable interactive analysis, slicers were added for Department, Job Role, Education Field, Tenure Bucket, Environment Satisfaction, and Years at Company.

Visuals and Dashboard Pages

Page 1: Overview
This page includes KPI cards showing the highest attrition rate, lowest average income, lowest department satisfaction, and highest job satisfaction. A pie chart displays the distribution of attrition across departments. A stacked bar chart shows attrition by education field.

Page 2: Income and Job Satisfaction
This page includes a dual-axis chart comparing monthly income and job satisfaction across departments. A clustered bar chart shows average income and job satisfaction per job role.

Page 3: Tenure-Based Insights
This page includes small multiples showing attrition by department across different tenure buckets (0-1, 2-3, 4-5, 6-10, 11-20, 20+ years). Another chart compares projected attrition and job satisfaction by department using a bar and line chart combination. This chart shows satisfaction as a strong predictor of future attrition.

Key Findings

Attrition Insights
The highest attrition rate, at 21 percent, was observed among employees with low satisfaction and short tenure of 0-1 years.
Departments with the lowest average income, such as Sales, experienced relatively higher attrition.
Employees with job satisfaction levels above 3.25 had significantly lower projected attrition.
Employees with 11 to 20 years of tenure showed moderate attrition but consistently high satisfaction.

Projected Attrition
Projected attrition rates drop from 9.3 percent among low-satisfaction departments to as low as 1.5 percent in high-satisfaction departments. The greatest potential impact lies in increasing satisfaction for early-tenure employees.

Strategic Implications
Onboarding strategies should be strengthened to address high attrition in the first year.
Job satisfaction programs should be developed to retain talent, especially in high-stress departments.
Income adjustments could reduce turnover in low-income roles.
Specific departments like HR and R&D showed unique patterns; HR had high early attrition, while R&D reported lower satisfaction across all tenures, suggesting department-level interventions.

Future Enhancements
Add predictive modeling using Python to validate projected attrition.
Incorporate qualitative survey data such as work-life balance and management quality for deeper insights.
Integrate the dashboard with Power BI Gateway to enable real-time HR reporting.
Set up Power Automate alerts for high-risk attrition cases based on satisfaction and tenure filters.

Tech Stack
Power BI was used for data modeling, dashboard development, and DAX-based analysis.
DAX formulas were used to create calculated measures and columns.
The dataset was imported from Excel or CSV format for analysis.
