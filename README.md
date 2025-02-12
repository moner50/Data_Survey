# Data_Survey
# Power BI - Data Professional Survey Analysis

## Project Overview
This project analyzes survey data from data professionals using Power BI. The goal is to provide insights into salaries, job satisfaction, and industry trends.

## Data Explanation

| **Category**         | **Column Name**                                           | **Description**                                      |
|----------------------|----------------------------------------------------------|------------------------------------------------------|
| **Demographics**     | `Q9 - Male/Female?`                                      | Respondent's gender                                 |
|                      | `Q10 - Current Age`                                      | Respondent's age                                    |
|                      | `Q11 - Which Country do you live in?`                    | Country of residence                               |
|                      | `Q12 - Highest Level of Education`                       | Highest educational qualification                   |
|                      | `Q13 - Ethnicity`                                        | Ethnic background                                  |
| **Employment**       | `Q1 - Which Title Best Fits your Current Role?`          | Job title (e.g., Data Scientist, Analyst)         |
|                      | `Q3 - Current Yearly Salary (in USD)`                    | Salary range (e.g., 0-40k)                         |
|                      | `Q7 - How difficult was it for you to break into Data?`  | Difficulty level of entering the data field        |
| **Job Satisfaction** | `Q6 - How Happy are you in your Current Position with the following?` | Ratings on management, learning opportunities, etc. |
| **Other**           | `Q8 - If you were to look for a new job today, what would be the most important thing to you?` | Job-seeking priorities (e.g., salary, remote work) |

## Data Cleaning Steps
1. **Job Title Cleaning**
   - Split `Q1 - Which Title Best Fits your Current Role?` by `(` to remove extra text.
   - Kept only the primary job title.

2. **Salary Processing**
   - Split `Q3 - Current Yearly Salary (in USD)` (e.g., `0-40k`) into two columns:
     - Minimum salary (e.g., `0`)
     - Maximum salary (e.g., `40,000`)
   - Calculated the **average salary** from both values.

## Dashboard Insights
- **Total Survey Participants**: Number of respondents.
- **Average Age**: Mean of `Current Age`.
- **Salary by Job Title**: Average salary grouped by `Job Title`.
- **Survey Distribution by Country**: Number of respondents per country.
- **Most Used Programming Language**: Python is the most used, mainly in data science.
- **Difficulty Breaking into Data Field**: Most respondents found it "Very Easy".



