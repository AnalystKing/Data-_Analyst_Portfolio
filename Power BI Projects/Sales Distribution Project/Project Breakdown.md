## Sales Distribution Project
### Project Overview
This data analysis project using the sales distribution dataset of a company aims to provide insight into sales trends and patterns across regions and through the year, top performing products as well as the top purchasing customers of the company. It also seeks to answer important qusetions as to whether the various company's targets are been met.  

### Data Sources
Sales_Distribution_file.csv: The primary dataset used for this analysis is the 'Sales_Distribution_file.csv' file containing important information about sales in the organization as well as the company's target. The dataset is sourced from [here](https://leanexcelsolutions.com/wp-content/uploads/2022/04/Sales-Distribution-Practice-File.xlsx)


### Tools
The primary tool used in this analysis is Power BI [(Download here)](https://www.microsoft.com/en-us/download/details.aspx?id=58494). Power BI was used for the following processes:
- Importing the data into Power BI
- Exploring, cleaning and formatting the data using Power Query editor
- Carrying out statistical analysis
- Visualizing the data and creating a dashboard
- Publishing and the sharing the dashboard

### Data Cleaning/Preparation
In the initial data preparation stage, we performed the following tasks;
- Data loading and inspection
- Checking formatting and handling missing values
- Data cleaning and formatting
- Creating calculated columns and measures 

### Exploratory Data Analysis (EDA)
EDA involved exploring the sales data to answer key questions, such as;
- What is the number of employees and attrition rate in the organization?
- What is the performance and satisfaction level of employees in the organization?
- What is the age and gender balance of employees across each department?
- How often did employees strive to improve their selves through training in the previous year?

### Data  Analysis
Some of the functions or syntax used during analysis in excel includes: 
- Current number of employees
```excel
=SUM(CF.current Employee column)
```

- Attrition rate
```excel
=(GETPIVOTDATA("Employee Count",$C$2)-GETPIVOTDATA("CF_current Employee",$A$2))/GETPIVOTDATA("Employee Count",$C$2)
```

- Average Age
 ```excel
  =AVERAGE(Age_column)
```

### Results/Findings
Some of the analysis results are as follows:
- There are currently **1,233** employees in the organization with the overall attrition rate of **16%**. About 237 employees have left the organization within the time scope of the dataset.
- The average performance rating of employees in the organization is **3** out of **5**. While the job and environment satiscation levels can be considered satisfactory or very good as majority of the employees rate it a **3** or **4** out of **4**.
- The average age of employees in the organization is **37** with most within the **25-34** and  **35-44** age brackets. There are **732** males and **501** females within the organization with the **R&D** department having the majority of the employees, both male and female.
- Over the course of the previous year, majority of the employees underwent training twice or thrice.

Here is a preview of the dashoard for reference:

![Dashboard](https://github.com/user-attachments/assets/47ddd0fb-91eb-4d72-8c16-3d6cdcb981d0)

To interact with the dashboard and apply filters, click here: [HR Data - Copy.xlsx](https://github.com/user-attachments/files/17045679/HR.Data.-.Copy.xlsx)

### Recommendation
Based on the analysis, we recommend the following actions;
- The sales department should be looked into as it recorded the highest rate of attrition of 21%.
- Some employees are due for promotion.

### Limitations
The dataset did not contain a date time column for reference on time period the data was collected. 

### Reference 
- Excel tutorial on [W3schools.com](https://www.w3schools.com/excel/index.php)



