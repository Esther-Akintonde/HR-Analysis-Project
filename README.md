# HR Analysis Project

### Project Overview
This data analysis project aims to provide insights into the Human resource data of a company for over one decade. By analyzing various aspects of the HR data, we seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the effect of human resource on the company's performance.

### Data Sources
HR Data: The primary dataset used for this analysis is the "Hr Analysis Dataset.xlsx" file, containing detailed Human resource information of each employee of the company.

### Tools
Ms Excel - Data Cleaning, Data Analysis and Data Visualization

### Exploratory Data Analysis
EDA involved exploring the Human Resource data to answer key questions, such as:

- What is the total number of employee since inception?
- What is the total number of current employee?
- What is the total number of terminated employee?
- What is the employee termination rate?
- What is the total salary paid?

### Data Analysis
Listed below are some Data Analytics Expression (DAX) used in PivotTable Analyze of MS Excel to answer key questions and generate insights from data.

1. Total Employee since inception
~~~Excel
=COUNT(Employee[ID_employe])
~~~
![image](https://github.com/user-attachments/assets/32aeb594-159d-461d-b86f-95db58bc0ae8)

2. Current Employee Head Count 
~~~Excel
=CALCULATE([Total Employee],Employee[Attrition]="No")
~~~
![image](https://github.com/user-attachments/assets/536f1697-9bcb-4a26-b0c4-b0a99ad96435)

3. Terminated Employee Count 
~~~Excel
=CALCULATE(Employee[Total Employee],Employee[Attrition]="yes")
~~~
![image](https://github.com/user-attachments/assets/b096c3d7-c4bf-4ef4-95ba-97a1d1a55def)

4. Total Salary Current Employee 
~~~Excel
=CALCULATE(SUM(Employee[Salary]), Employee[Attrition]="No")
~~~
![image](https://github.com/user-attachments/assets/378342a6-6cd1-442e-a2e8-a96a12f44f2a)

5. Total Salary all Employee 
~~~Excel
=SUM(Employee[Salary])
~~~
![image](https://github.com/user-attachments/assets/a816f3f5-b5b7-4eb2-bb08-da7e02618db4)

6. Employee Termination Rate 
~~~Excel
=[Termination]/[Head Count]
~~~
![image](https://github.com/user-attachments/assets/9520f49b-49f5-4e70-b90a-9be3f28ad466)

Results/Findings
The analysis results are summarized as follows:

1. Majoriy of the employee has a bachelors degree which is equivalent to 40% of the total employee.
2. We realized that the rate of Job satisfaction in the organization is very high, with low number of employee not satisfied with their job.
3. The highest number of employer termination was recorded in 2021 to be 53 with a termination rate of 44.17% which can be concluded to be the effect of Covid 19 outbreak in 2020.
4.  Majority of the Employees have a better worklife Balance at 62.1%, while others are good 



