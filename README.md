# HR Analytics and Employee Attrition Dashboard

An Excel-based analysis of employee attrition, built with Power Query, PivotTables, and an interactive dashboard.

## Problem Statement

The organisation has an overall attrition rate of 16.1% (711 leavers). This project identifies who is leaving, when, and why, so that HR can target retention action where it will have the most effect.

## Dataset

The IBM HR Analytics dataset covers 4,410 employees. It is supplied as three CSV files, merged on `EmployeeID`:

| File | Content |
|---|---|
| `general_data.csv` | Demographics, role, income, tenure, travel, attrition status |
| `employee_survey_data.csv` | Environment, job, and work-life balance satisfaction |
| `manager_survey_data.csv` | Job involvement and performance rating |

## Methodology

**Power Query**
1. Imported the three CSV files.
2. Merged `general_data` with the two survey files on `EmployeeID` (left join).
3. Handled missing values, removed duplicate records, and standardised categorical values.
4. Loaded the clean table into the workbook.

**Analysis and dashboard**
1. Built PivotTables for attrition by tenure, age, marital status, travel, satisfaction, department, job role, income, and performance rating.
2. Created a composite satisfaction score (Low: below 2.5).
3. Assembled an interactive dashboard from the PivotTables.

## Key Business Insights

| No. | Insight | Supporting evidence | Implication |
|---|---|---|---|
| 1 | Attrition is mainly a problem in the first two years. | Employees with 0-2 years' tenure leave at 29.8%, against 16.1% overall. They are 23% of the workforce but 306 of 711 leavers (43%). The rate falls to 13.8% at 3-5 years and 6.7% at 11-20 years. | Recruitment and training spend is lost early. Onboarding and early support are the biggest opportunity. |
| 2 | Young and single employees are the highest-risk group. | Ages 18-24 leave at 39.2% (114 of 291) and ages 25-34 at 20.2%. Staff under 35 are 44% of the workforce but 63% of leavers (450 of 711). Single employees leave at 25.5%, against 12.5% for married and 10.1% for divorced staff. | Without visible growth paths and support, early-career staff will continue to leave. |
| 3 | Frequent business travel is strongly linked to attrition. | Frequent travellers leave at 24.9%, three times the 8.0% of non-travellers. They are 19% of staff but 29% of leavers (207 of 711). New joiners (0-2 years) who travel frequently leave at 47% (198 employees). | Travel demands are hardest on people who have not yet built loyalty or a support network. |
| 4 | Low satisfaction predicts exit. | Low-satisfaction employees leave at 23.4%, against 6.5% for High, about 3.6 times higher. Those scoring 1 on work-life balance leave at 31.4% (75 of 239); those scoring 1 on environment satisfaction leave at 25.2%. | Survey results give HR an early warning, so at-risk employees can be supported before they resign. |
| 5 | Attrition is concentrated in specific groups. | Human Resources has an attrition rate of 30.2% (57 of 189), twice that of R&D (15.7%) and Sales (15.0%). Research Director has the highest role rate at 23.8% (57 of 240); Manufacturing Director the lowest at 11.0%. | Targeted action will work better than company-wide measures. These groups are small, so rates should be interpreted with care. |
| 6 | Pay does not explain attrition, and the pay structure looks flat. | Attrition ranges from 12.3% to 17.5% across income bands with no clear pattern. Leavers earn only 6% less on average (61,683 against 65,673). Average pay across roles ranges only from about 58.5K to 69.2K, and Managers (63.4K) earn less than Laboratory Technicians (66.3K). | Pay rises alone are unlikely to cut attrition. The narrow gap between roles may weaken the incentive to progress and should be reviewed. |
| 7 | Top performers are not better retained. | Employees rated 4 for performance leave at 18.1% (123 of 678), slightly above the 15.8% of those rated 3. | High performers are being lost at least as quickly as average performers, which affects capability and succession. |

## Recommendations

1. Strengthen onboarding and early-tenure support, particularly during the first two years.
2. Create visible career paths for employees under 35.
3. Review travel expectations for new joiners and frequent travellers.
4. Use satisfaction survey results as an early-warning indicator.
5. Investigate the Human Resources department and the Research Director role directly.
6. Review the pay structure and the progression incentive between roles.
7. Introduce retention measures for high performers.

## Tools

Microsoft Excel, Power Query, PivotTables, and Excel dashboard features.

## Repository Contents

- `hr_analytics_dashboard.xlsx`: the complete workbook (cleaned data, analysis, dashboard).

## Note

The dataset is the publicly available IBM HR Analytics dataset and contains no real employee information.
