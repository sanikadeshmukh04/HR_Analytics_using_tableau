# HR_Analytics_using_tableau
Interactive Tableau dashboard analyzes employee attrition using the HR-Employee-Attrition dataset (1,470 records, 35 attributes). It helps HR teams see who is leaving and why, supporting data-driven retention decisions.

## Objective
To identify the key drivers and patterns behind employee attrition so HR and management can make data-driven retention decisions.

## Dashboard Components

# The HR Analytics Dashboard combines seven worksheets:

**1.KPI Summary:** headline metrics such as total employees, attrition count, attrition rate, active employees and average age.

**2.Attrition by Gender:** compares attrition between male and female employees.

**3.Department-wise Attrition:**  a pie chart showing how attrition is distributed across departments.

**4.Education Field-wise Attrition:** shows which educational backgrounds see the most turnover.

**5.Job Satisfaction Rating:** a heatmap of job role against satisfaction score.

**6.No. of Employees by Age Group:** a histogram of the workforce age distribution.

**7.Attrition Rate by Gender across Age Groups:** a pie chart breaking down attrition by gender within each age band.

# Calculated Fields
1.Age Group: buckets employees into 18–30, 31–40, 41–50 and 51–60.

2.Attrition Count: IF [Attrition] = 'Yes' THEN 1 ELSE 0 END

3.Attrition Rate: SUM(Attrition Count) / SUM(EmployeeCount)

4.Active Employee: SUM(EmployeeCount) − SUM(Attrition Count)

5.Age (bin) + Bin Size parameter: a user-adjustable bin size (2–10) for the age histogram.
