# 📊 Employee Retention

## 1. Overview
This project explores the factors affecting employee retention and aims to provide insights that can help organizations reduce turnover. By analyzing HR and workforce-related data, we identify trends, key drivers of attrition, and patterns among employees who are likely to stay or leave.

## 2. Data Source
Dataset: [Kaggle: HR Employee Retention]([https://www.kaggle.com/datasets](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction/data))  
Contains 14999 total values

## 3. Tools & Libraries 🛠️
- **Python** (Pandas, Matplotlib, Seaborn)
- **Jupyter Notebook** for data analysis and visualization

## 4. Analysis & Insights 🔍
## 4.1 Insight:
### 4.1.1: Insights about outliers

- Outliers only 2.04%, so it doesn’t have a significant impact on the data.   

### 4.1.2: Insights about "Department" and "Left". 

- Almost people in Sales, Technical, Support spend a lot of time in company but the salary is still 

#### I figure out that 3 departments have the highest attribution so i dig deeper into it.
#### 4.1.2.1: Insights about "Department" and "Salary"

- 20% of all employees with low salaries and 14.6% of all employees with medium salaries left the company.

#### 4.1.2.2: Insight about 'Department' and 'Average_monthly_hours' 

- Employees in the Sales, Technical, and Support departments tend to work longer hours.

#### 4.1.2.3: Insight about "department" and "Promotion_last_5years"
- Of 824 employees with over 5 years at the company, only 5% were promoted. Among the 783 not promoted, 14% left, while 100% of promoted employees stayed.

#### 4.1.2.4: Insight about "department" and "Number_project"

- The Sales department consistently handles the most projects, averaging 3.67%–10.61% more than the second-highest team.

- Employees with low salaries and more than 5 projects have a very high turnover (left rate). These employees also spend more years at the company, but still leave at a high rate → suggesting possible burnout or underpayment.

### 4.1.3: Insight about 'Satisfaction_level' and 'Left'

- Satisfaction_level is lower, Employees tend to left the company

### 4.1.4: Insight about 'Last_evaluation' and 'Left'

- Last evaluation is lower than 0.6 make employees tend to left the company

### But i figure out Last evaluation is greater than 0.8 still make employees tend to left the company ? so i dig deeper and have a insight:
#### 4.1.4.1:

- Employees with high evaluation scores who experienced both high workload and insufficient rewards (e.g., low salary or no promotion) were more likely to leave the company.

### 4.1.5: Insight about "Average_monthly_ hours" and "Left"

- Employees who work between 130–160 hours and those who work between 230–280 hours per month tend to show a higher intent to leave the company

### 4.1.6: Insight about correlation

- Satisfaction_level is impacted Negatively by Number_project, time spend company and left. Number of project is impacted negatively by Satisfaction_level, salary

### 4.1.7: Result of the hypothesis testing

- The results of the hypothesis testing: With z-scores of -2.58 for promotion and 8.02 for salary, both values fall within the rejection regions of the standard normal distribution. Therefore, we reject the null hypotheses for both cases. The corresponding p-values of 0.009 (promotion) and < 0.0001 (salary) are both less than the significance level of 0.05. These results provide strong statistical evidence of significant differences in attrition rates related to promotion status and salary level.

## 4.2 Proposal
- Review salary, especially for high-performing and long-tenure employees.

- Recognize and promote employees who have spent many years and contributed significantly.

- Rebalance workloads, particularly in the Sales department.

- Monitor working hours to avoid burnout, especially in extremes.

- Employees with last evaluation > 0.8 should be prioritized for rewards or stretch assignments.

- Track promotion eligibility for employees with >3 years of service.

- Cap the number of high-stress projects per employee (e.g., max 5 projects/month).

## How to Run 🖥️
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/Employee-Retention.git
