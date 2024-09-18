## HR Data Analysis And Dashboard
### Project Overview
This data analysis project using a HR dataset aims to provide insight into attrition trends, job performance and satifaction levels as well as employee self development rate. It also seeks to analyze the gender, marital and age balance of employees in the organzation. 

### Data Sources
HR Data: The primary dataset used for this analysis is the 'HR_Data.csv' file containing important information about each employee in the organization. The dataset is sourced from [here](https://docs.google.com/spreadsheets/d/17zaiJnUOnLdHROWLZYcVlpMJ08wh-Bou/edit?gid=115883679#gid=115883679)


### Tools
The primary tool used in this analysis is Excel [(Download here)](https://microsoft-excel.en.softonic.com/download). Excel was used for the following processes:
- Extracting the data
- Cleaning and exploring the data
- Analyzing the data
- Visualizing the data and creating a dashboard.

### Data Cleaning/Preparation
In the initial data preparation stage, we performed the following tasks;
- Data loading and inspection
- Checking formatting and handling missing values
- Data cleaning and formatting

### Exploratory Data Analysis (EDA)
EDA involved exploring the employee data to answer key questions, such as;
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


