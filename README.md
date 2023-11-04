# Project 1 : Ecommerce Sales Analysis

## Table of contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Explanatory Data Analysis](#explanatory-data-analysis)
- [Data Analysis](#data-analysis)
- [Findings](#findings)
- [Dashboard](#dashboard)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
  

### Project Overview
---
This data analysis aims to provide insights into sales performance of an e-commerce company over the past year. By analysing various aspects of the sales of the sales data set, i seek to identify trends, make data driven recommendations, and gain a deeper understanding of the company's performance.

### Data Source

Sales Data: Data Source
The data used for this analysis was queries written on a Relational Database management system(MySQL) to return the necessary data containing detailed information about each sales made by the company.

### Tools

- Excel - Data Cleaning
- MySQL Server - Data Analysis
- Tableau - Creating Report

### Data Cleaning

1. Formatted the data.
2. Removed duplicates.
3. Remove blanks.
4. Removed null values.
5. Used text to column function to correct date with error.
6. Used trim fuction to remove unecessary spaces in the data.

### Explanatory Data Analysis 

EDA involve exploring the sales data to answer key questions, such as:

- What is the overall sales trend?
- What products are the top sellers?
- What are the peak sales period?
- What region made the most sales?
- What segment of the customer was sales made the most?
- What was the most used shipment mode for sales?
- What state made the most sales? 

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
1. The company's sales have been fluctuating past months, with a noticale as peak in november.
2. Phones are the top seller with an impressive $105,340.52 followed closely by chairs with Reasonable $95,554.35 made from sales.
3. Within the segment pool, an unbeliveable $331,904.70 was made from consumer.
4. The peak sales period is november,making an amazing $118,447.83.
5. The west region comes out top, making a 34.11% of the total sales accross all region.
6. Interms of shipment mode, as espected standard class made an increadibles $395,603.52 from sales.
7. California comes our top as the best performing state with a remarkable $146,388.34 made.

### Dashboard

![Ecommerce Sales Dashboard 2020](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/d11245a4-450d-4ba0-bb9c-a5d092c2f15b)

### Recommendations

Based on the analysis, i recommend the following actions:
- invest in marketing and promotion during the peak sale period.
- Focus on expanding  and promoting products with the lowest sale.
- implement a customer segmentation strategy to target "home office" customers.
- Focus more marketing and promotion stategies on eastern region.
- Priority should be places same day delivery customer by maaking sure that shipment gets to the customer, at the promised time.

### Limitations

i had to remove all null values from the revenue column because they would have affected the accuray of my conclusion from the analysis.


# Project 2: Sales Analysis

## Table Of Content

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Explanatory Data Analysis](#explanatory-data-analysis)
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
              
### Data Cleaning

In the initial data preparation phase, we performed the following tasks:
1. Data Loading and Inspection
2. Formatted the data
3. Used Vlook up to look up the values of other tables(company and representatives) in the main excel sheet as the excel file contained two sheets.
4. Data Formating
5. Used Trim function to remove unecessary spaces
6. Used Upper case funtion
7. Removed duplicates

### Explanatory Data Analysis

- What is the overall sales trend
- What region made the most sales
- Who is the best performing sales rep
- Which product are the  top sellers
- What are the peak sales period
- Which companies are the top seller

### Findings

1. There is an increase in sales for the first four months of the year and there comes a decline in sales for the last two months.
2. in terms of sales made by each region,all companies combined made their best sales in the south region with a enviable $211,900 made from sales.
3. marc williams is the best performing sales rep accross all companies with a noticeable $123,885 made from sales with eric jones following up closely at $91,015.
4. Black Energy makes up 14% of the total sales in terms of model and color collectively at best with total sales of $86,800
5. The peak sales period is april with an impressive $126,565 made from sales.
6. The best performing company over the month is Bankia Ltd sitting at the top with a total sales of $114,825.

### Dashboard

![Sales Analysis Dashboard](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/5d43a348-7206-46c9-be75-9c3c7c4cc59e)

### Recommendations

- invest in marketing and promotion during the peak sale period
- give sales reps incentives and commission to encourage sales
- focus more marketing strategies on the  north region to improve sales
- focus on filling and expanding the stores with no products to boost sales

### Limitations

I had to remove unecessary blanks that would have distorted the accuracy of my analysis and conclusions.


# Project 3: Health Insurance Analysis

## Table Of Contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Explanatory Data Analysis](#explanatory-data-analysis)
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
2.In terms of age and gender,men between the age of 48-57 take their health insurance very seriously as they spend more on insuring their health.
3. The region that is most involed in health insurance is the southeast region.
4. Non-smokers spends more on insuring their health.
5. People who weight between 25.96-35.96 are more actively involved in health insurance.
6. Couples with no children show the most interest in insuring their health.

### Dashboard

![Capture 6](https://github.com/DarlingtonAlban/Darlington_Portfolio/assets/141925298/9ce062a7-3f26-46cb-9f6b-b07092772ca1)

### Recommendations

Based on the analysis, i advice the following action:
1. smokers should spend health insurance more seriously as they are pron to health issues.
2. couples with children should prioritise the health of their children.

### Limitations

i had to remove the zeros on the charges column which would have affected the accuracy of my analysis and conclusion.
