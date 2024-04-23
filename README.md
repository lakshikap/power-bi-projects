# power-bi-projects
Power BI Projects are in progress. Here you will see the report and dashboard creation activities/files that lead to the exercises and projects that are upcoming.

Exercise 1:  
- Imported the dataset and opened it in Power Query. Prepared the data by checking errors and inconsistencies. For example, the expense type column had some spelling and punctuation errors which were replaced with correct values.  
- The Project names were not uniform, do they were made consistent using replace function.  
- Moreover, the Currency column had some missing values. So, based on the amount, created a new custom column and added a condition:
- Condition: amount >= 1000, = LKR; amount < 1000, = USD; else = EURO.
- Formula: (if [Currency] = null and [Amount] >= 1000 then "LKR" else if [Currency] = null and [Amount] < 1000 then "USD" else [Currency] ).
- Then normalized the amount column into LKR based on the currency column.  
- Created a measure to calculate the sum of reimbursed amount in LKR.  
- Used the calculate function and check the total reimbursed amount for Project_B.  
- Created a measure to check the count of declined requests.  
- Created a slicer visual for the Project and employee.  
- Created a bar chart for employees and reimbursement amount.  
- Created a pie chart for Project vs reimbursement amount.  

Exercise 4:  
Datasets:  
1. fact_sales_Iphone14.csv  
2. fact_sales_Iphone15.csv  
3. dim_stores.csv

Tasks:  

1. Reviewed the data (fact_sales_Iphone14andfact_sales_Iphone15).   
2. Compared metrics - iPhone14sales and iPhone15sales.   
3. Calculated the variance (absolutedifferencevalue) between the iPhone15 sales and iPhone14 sales for the identified metrics. ABS([Iphone 15 Sales]-[Iphone 14
Sales]).  
4. Calculated the variance (inpercentage) between the iPhone15sales and iPhone14 sales for the identified metrics. [([Iphone 15 Sales]-[Iphone 14 Sales])/[Iphone
14 Sales].  
5. Provided a complete report of the difference in numbers between the iPhone15 sales and iPhone 14 sales data across the top 10 countries.  

