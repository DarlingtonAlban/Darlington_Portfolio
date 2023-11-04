# Project 1 : Ecommerce Sales Analysis

## Table of contents

- [Project Overview](#project-overview)

### Project Overview

This data analysis aims to provide insights into sales performance of an e-commerce company over the past year. By analysing various aspects of the sales of the sales data set, i seek to identify trends, make data driven recommendations, and gain a deeper understanding of the company's performance.

### Data Sources

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

### Recommendations

Based on the analysis, i recommend the following actions:
- invest in marketing and promotion during the peak sale period.
- Focus on expanding  and promoting products with the lowest sale.
- implement a customer segmentation strategy to target "home office" customers.
- Focus more marketing and promotion stategies on eastern region.
- Priority should be places same day delivery customer by maaking sure that shipment gets to the customer, at the promised time.

### Limitations

i had to remove all null values from the revenue column because they would have affected the accuray of my conclusion from the analysis

