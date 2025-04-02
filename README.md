# Jobs-and-Salaries-in-Data-Roles
Analyzed different data jobs and their salaries. Used SQL to create queries and Tableau to visualize those queries

# Project Overview
This project explores a global dataset of job titles, locations, company sizes, and salaries in the data and tech industry. Using a combination of SQL for analysis and Tableau for data storytelling, the goal was to uncover insights around job demand, compensation trends, and role distribution across industries and geographies.

The final output is an interactive Tableau dashboard that allows decision-makers to visually explore high-paying roles, salary disparities by experience, and how geography or work setting impacts compensation.

# Background and Purpose
With remote work reshaping job markets and data roles becoming more vital across industries, understanding how salary, location, job type, and experience intersect is key for:
* Job seekers navigating their career paths
* Employers setting competitive compensation packages
* Analysts and workforce planners predicting hiring trends

# Data Overview
The dataset includes the following fields:
* work_year
* job_title, job_category
* salary_currency, salary_in_usd, salary_in_local
* employee_residence, employement_type, experience_level
* work_setting, company_location, company_size

# Methods and Tech Stack
* SQL (PostgreSQL): used for data wrangling, aggregation, and EDA (CTEs, window functions, case statements, aggregate functions)
* Tableau: used for visualizing the queries and storytelling
* pgAdmin4: used for executing SQL queries and validating table structure

# Dashborad Features
https://public.tableau.com/app/profile/jordan.aparece/viz/JobsandSalariesinDataScience_17435482810850/Dashboard1

Key Visualizations:
🔝 Top 10 Most Common Job Titles

💸 Average Salary by Experience Level

🌍 Highest Paying Countries

👨‍💻 Top 10 Paying Roles (with over 100 entries)

🏢 Salary Distribution by Company Size

🧭 Remote vs In-Person Salary Comparison

📈 Salary Trend by Experience Level Over Time

# Key Recommendations
* Executive roles lead in pay, but volume is low
  * Executive roles top the salary scale, but senior and mid-level roles dominate the market
* Remote jobs pay slightly less on average
  * Remote jobs offer flexibility but trend lower in compensation compared to in-person roles
* Smaller companies underpay significantly
  * There's a strong correlation between company size and salary - larger companies pay more on average
* Job title inflation is real
  * Certain high-salary job titles only appear a few times in the data - filtering by volume and removing
    outliers provides more reliable insights

# Challenges Encountered
The main challenge of the dataset was dealing with outliers. Outliers in this are considered job titles that are more "obscure", such as titles that are not as common as others. Roles such as these skewed the data. For example, there was one instance of a job in Qatar which had a USD salary of $300,000. Including this would severely skew the data despite it only being one record. Similarly, there are only 3 record with the title "Data Analytics Lead", one of which has a salary of $405,000. Again, including this would severely skew the data, so removing outliers as such allows for more reliable insights.
