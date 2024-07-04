# Project 1 : Ecommerce Sales Analysis

## Table of contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Findings](#findings)
- [Dashboard](#dashboard)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
  

### Project Overview
---
This data analysis aims to provide insights into sales performance of an e-commerce company over the past years. By analysing various aspects of the sales data set, i seek to identify trends, make data driven recommendations, and gain a deeper understanding of the company's performance.

### Data Source

Sales Data: Data Source
The data used for this analysis was queries written on a Relational Database Management System(MySQL) to return the necessary data containing detailed information about each sales made by the company.

### Tools

- Excel - Data Cleaning
- MySQL Server - Data Analysis
- Tableau - Creating Report

### Data Cleaning

1. Exported the data from mysql server to excel
2. Formatted the data.
3. Removed duplicates.
4. Removed null values.
5. Used text to column function to correct date with error.
6. Used trim fuction to remove unecessary spaces in the data.

### Exploratory Data Analysis 

EDA involve exploring the HR data to answer key questions, such as:

- What is the company sales over the years?
- Which of the company's product sold the most?
- Which segment of the company made more sales?
- What is the best performing month of sales for the company?
- Which region came out top in terms of sales?
- Which mode of shipment realized the most sales?
- Which state is the best performing state in terms of sales?
  
### Data Analysis

```sql
Select o.order_date, o.row_id, o.order_date, o.shipment_mode,
       c.customer_id, c.segment, c.country, c.city, c.state,c.postal_code,c.region
       p.product_id,p.category,p.product_name,p.sales
       From Orders o
       Left Join customer c
       On o.customer_id = c.customer_id
       Left Join Products p
       On o.order_id = p.order_id
```

### Findings

The analysis results are summarized as follows:
1. The company's sales have been flunctuating for the past months, with a noticeable peak in november.
2. Phones are the top seller with an impressive $105,340.52 followed closely by chairs with a reasonable $95,554.35 made from sales.
3. Within the segment pool, an unbeliveable $331,904.70 was made from consumer.

![Sales By sub-categories](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/78334495-3b34-4a89-998f-7c91c0d96941)


![Sales By Segment 2020](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/be8ccd57-3767-44a7-a4f0-e9b12debfbaf)

  
4. The peak sales period is november,making an amazing $118,447.83.
5. The west region comes out top, making a 34.11% of the total sales accross all region.

![Sales By Order Date](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/c74925b7-ae29-4910-ae65-3e0c1705df41)


![Sales By Region 2020](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/e9c069c6-8341-4138-b70e-354babe919dc)


6. In terms of shipment mode, as expected standard class made an increadible $395,603.52 from sales.
7. California comes out top as the best performing state with a remarkable $146,388.34 made.

![Sales By Shipment Mode 2020](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/f817baba-7e1e-43ea-9200-1803dc3f1cdf)

![Sales By State](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/2d899463-9109-4642-883d-e11dfa73f04e)

### Dashboard

![Ecommerce Sales Analysis Dashboard 2020](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/5edbb2a5-de4c-449a-8386-dad55118ef23)

### Recommendations

Based on the analysis, i recommend the following actions:
- invest in marketing and promotion during the peak sale period.
- Focus on expanding  and promoting products with the lowest sale.
- implement a customer segmentation strategy to target "home office" customers.
- Focus more marketing and promotion stategies on eastern region.
- Priority should be places on same day delivery customer by maaking sure that shipment gets to the customer, at the promised time.

### Limitations

i had to remove all null values from the revenue column because they would have affected the accuray of my conclusion from the analysis.

# Project 2: HR Analysis

## Table Of Content

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Findings](#findings)
- [Dashboard](#dashboard)
- [Limitations](#limitations)

### Project Overview
---
This data analysis project aims to provide insight into the HR recruitment performance of the company over the years, By analysing various aspects of the hr data, we seek to identify trends, make data driven decision and recommendation, and gain understanding of the hr perfomances.

### Data Source

HR Data: the primary dataset used for this analysis is the "HR_dataset.excel" file given to me by a friend, containing detailed information about employees perfomance in the company.

### Tools

- PowerBi(Creating Report)
- PowerQuery(Data Cleaning)
- DAX Function(Employee Head Count)

### Data Cleaning

1. Exported the data excel to powerbi
2. Formatted the data
3. Removed duplicates
4. Removed Unwanted Columns
5. Replaced null values

### Exploratory Data Analysis 

EDA involve exploring the HR data to answer key questions, such as:

- Which department reacives the most salary?
- What is the number of candidates recruited each year?
- What is the number of employees according to their marital status?
- What is the ratings of the employee according to their perfomance score?
- Which gender has the most employee?
- Which state has the most employees?

### Findings

1. The product department of the company received the most salary at a whooping sum of $12.5m over the years.
2. 2011 has the most employee intake with a total of 83 candidates.

![HR Salary By Department](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/1fda3c49-ca52-448f-b22a-7e87852da6ee)

![HR Candidate Recruitment By Year](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/dfc894e8-0f0f-4358-a820-36c862a2a666)

3. Single makes up 44.05% of the total employees as regards marital status.
4. The company record the highest number of employees who fully meets their target at a total of 243 candidates.

![HR Candidate By Marital Desc](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/9df9ca2b-b8f9-4904-b44a-76ddcc835679)

![HR Candidate By Perfomance Score](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/d75bbaa0-a448-4457-813d-bb7fa6f056c7)

5. The male employees makes up 43.41% of the total employees while the female employees makes up 56.57% of the total employees gender wise.
6. Employees from texas received the most salary at a combined $222,427.

![HR Candidate By Sex](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/949599d4-d69e-4d51-89f8-aca4a8ad2af0)

![HR Candidate By State](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/ab581701-c070-4421-bb6c-45cd24c89e5e)

### Dashboard

![HR Dashboard](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/f028ce5c-70c1-4545-83e8-4923c72590d2)

### Limitation
1. I had to delete some columns which would have affected the accuracy of my analysis
2. I had to replace null values with zero avoid incosistency in my analysi


# Project 3: Sales Analysis


## Table Of Content

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Findings](#findings)
- [Dashboard](#dashboard)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

### Project Overview
---
This data analysis project aims to provide insight into the sales performance of a group of companies over the months, By analysing various aspects of the sales data, we seek to identify trends, make data driven decision and recommendation, and gain understanding of the companies perfomances.

### Data Source

Sales Data: the primary dataset used for this analysis is the "sales_data.excel" file from my google data analytics project, containing detailed information about each sales made by each company.

### Tools

-Excel - For Data Cleaning
-Tableau - For Creating Report
              
### Data Cleaning/Preparation

In the initial data preparation phase, we performed the following tasks:
1. Data Loading and Inspection
2. Formatted the data
3. Used Vlook up to look up the values of other tables(company and representatives) in the main excel sheet as the excel file contained two sheets.
4. Data Formating
5. Used Trim function to remove unecessary spaces
6. Used Upper case funtion
7. Removed duplicates

### Exploratory Data Analysis

- What is the overall sales trend?
- What region made the most sales?
- Who is the best performing sales rep?
- Which product are the  top sellers?
- What are the peak sales period?
- Which companies are the top seller?

### Findings

1. There is an increase in sales for the first four months of the year and there comes a decline in sales for the last two months. The peak sales period is april with an impressive $126,565 made from sales. 
2. in terms of sales made by each region,all companies combined made their best sales in the south region with a enviable $211,900 made from sales.

![Sales By date](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/35185640-4787-437e-ac3a-1d1d13b89be1)

![Sales By Region](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/722847e9-3827-4622-9cae-30e42ec9051f)

3. marc williams is the best performing sales rep accross all companies with a noticeable $123,885 made from sales with eric jones following up closely at $91,015.
4. Black Energy makes up 14% of the total sales in terms of model and color collectively at best with total sales of $86,800

![Sales By Sales Rep](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/595da6c0-88e6-44a0-ac06-c6bac7448fc5)

![Sales By Model   Color](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/150ff607-44d1-44ba-b21c-1865aa949b22)

5. The best performing company over the month is Bankia Ltd leveling above all other company with a total sales of $114,825.

![Sales By Company](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/9676996c-4fb0-4f7b-aff9-c7f56e9bbec2)

### Dashboard

![Sales Analysis Dashboard - Copy](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/83310784-11e5-47a5-94e2-22aac84411c6)

### Recommendations

- invest in marketing and promotion during the peak sale period
- give sales reps incentives and commission to encourage sales
- focus more marketing strategies on the  north region to improve sales
- focus on filling and expanding the stores with no products to boost sales

### Limitations

I had to remove unecessary blanks that would have distorted the accuracy of my analysis and conclusions.


# Project 4: Health Insurance Analysis

## Table Of Contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Results](#results)
- [Dashborad](#dashboard)
- [Recommendations](#recommendations)
- [LImitations](#limitations)

### Project Overview
---
this data analysis project aims to provide insights into the amount spent on health insurance by individuals and families over the years.
By analysing various aspect of the health insurance data set, i seek to identify trends and pattern and gain deeper understanding of how people prioritize their health.

### Data Source

The primary dataset used for this analysis "insurance.csv" file was downloaded from kaggle, containing detailed information about amount spent on health insurance by individuals and families.

### Tools

1.Excel - (Data Cleaning,Data Analysis & Creating Report)

### Data Cleaning

In the initial data preparation phase, we performed the following task:
1. Data Formating.
2. Removed Duplicates.
3. Trimmed the data to avoid unecessary spaces.
4. Used Upper case function for the data.
5. Handled missing values.
6. Used "isnumber" function to confirm if the columns with numerical values of the data are error free.
7. Used the "find and replace" function to change the indication of "yes" and "no" for the smoker column to
  "smoker" and "non-smoker" respectively.

### Exploratory Data Analysis
EDA involved exploring the health insurance data to answer key question, such as:

- What is the total amount spent by individuals and families on health insurance combined.
- Which gender and the age range spent more on health insurance simultaneously.
- Which region spent more on health insurance.
- who is more involved in health insurance between smokers and non-smokers.
- the amount people of a various weight range sepnd on health insurance.
- Which couples with children spent more on health insurance.

### Results

1. From the data below it shows that people spend alot of money to insurance their health, meaning that people take their health very seriously as the old saying goes, health is wealth.
2. In terms of age and gender,men between the age of 48-57 take their health insurance very seriously as they spend more on insuring their health.
3. The region that is most involved in health insurance is the southeast region.

![Insurance By Age   Sex](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/d44f636b-f2a9-4cf0-9bf8-5098b995f04b)

![Insurance By Region](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/c087e1fa-de45-466d-8f95-7c6c9a94f2fc)

4. Non-smokers spends more on insuring their health.
5. People who weight between 25.96-35.96 are more actively involved in health insurance.

![Insurance By Smoker Status](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/3301e98f-1109-4c8a-bdbd-872592e48456)

![Insurance By Weight](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/9c2351f5-2f1f-49ec-a681-fd686c8cec2f)

6. Couples with no children show the most interest in insuring their health.

![Insurance By Children](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/089926db-9971-40b1-b16f-d3b5d95509d4)

### Dashboard

![Insurance Dashboard](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/44bc1865-93ba-4db8-b766-d39507da9aa0)

### Recommendations

Based on the analysis, i advice the following action:
1. smokers should spend more health insurance more as they are pron to health issues.
2. couples with children should prioritise the health of their children.

### Limitations

i had to remove some missing values on the charges column and the weight column which would have affected the accuracy of my analysis and conclusion.
