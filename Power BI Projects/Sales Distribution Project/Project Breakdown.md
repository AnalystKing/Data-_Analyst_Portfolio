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
- Creating a dedicated date column and hierarchy

### Exploratory Data Analysis (EDA)
EDA involved exploring the data to answer key question, such as;
- What is the total sales for the year?
- Which products are the best selling products?
- Who are the top 3 purchasing customers?
- Are we meeting our monthly targets?

### Data  Analysis
Some of the functions or syntax used during analysis in Power BI includes: 
- Creating a custom column to calculate sales
```DAX
= Table.AddColumn(#"Changed Type", "Actual", each [#"UNIT PRICE ($)"]*[QUANTITY])
```

- Creating a dedicated month column
```DAX
= Table.AddColumn(#"Inserted Week of Month", "Month", each Date.Month([DATE]), Int64.Type)
```

- Creating a dedicated Week of Month column
```DAX
= Table.AddColumn(#"Added Custom", "Week of Month", each Date.WeekOfMonth([DATE]), Int64.Type)
```

- Craeting a dedicated Week of Year column
```DAX
= Table.AddColumn(#"Inserted Day", "Week of Year", each Date.WeekOfYear([DATE]), Int64.Type)
```

### Results/Findings
Some of the analysis results are as follows:
- The company made over **985,000** sales during the year.
- The top selling product is **Product30** with over **57,000** sales. The next best selling products are **Product41** and **Product24** respectively. The top 10 productsare displayed on the dashboard.
- The top purchasing customers are **Customer33**, **Customer22** and **Customer23** respectively.
- Monthly targets were reached in only 4 months. **January, July, October** and **December**. Sales in other months were below their respective monthly targets.

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



