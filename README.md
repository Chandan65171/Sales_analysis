# Sales_analysis
# AltiQ Hardware Sales Analysis - SQL

## Overview
This project conducts sales analysis for AltiQ Hardware Company, an electronic hardware manufacturer, utilizing SQL queries. The aim is to provide insights into sales trends, customer behavior, and product performance directly from the company's SQL database.

## Sample_Queries

Q1). Show distrinct product codes that were sold in chennai 
➡️ select distinct product_code from transactions where market_code='Mark001';

Q2). Show transactions where currency is US dollars  
➡️ select * from transactions where currency='USD';

Q3). Show transactions in 2020 join by date table 
➡️ select t.* , d.* from transactions as t join date as d on d.date=t.order_date where year=2020;

Q4). Show total revenue in year 2020 
➡️ SELECT 
    SUM(transactions.sales_amount) as  revenue
FROM
    transactions
        INNER JOIN
    date ON transactions.order_date = date.date
WHERE
    date.year = 2020
        AND transactions.currency = 'INR'
        OR transactions.currency = 'USD';

  ➡️ etc.
        
Executed all SQL queries using a preferred SQL client or command line.

 ## Aim
 ➡️ This project aims to provide insights into:
 💠 Sales performance: Overall sales trends, top-performing products and regions.
 💠 Customer behavior: Identify buying patterns and key customer segments.
 💠 Market analysis: Understand market trends and competitor performance (if data available).
 💠 Improve sales strategies and identify new growth opportunities.
 💠 Optimize product offerings and marketing campaigns.
 💠 Make data-driven decisions for better resource allocation.

##  Tools used
 💠 SQL (Query Language)
 💠 MySQL (Database) 
