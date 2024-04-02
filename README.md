# Sales_analysis
# AltiQ Hardware Sales Analysis - SQL

## Overview
This project conducts sales analysis for AltiQ Hardware Company, an electronic hardware manufacturer, utilizing SQL queries. The aim is to provide insights into sales trends, customer behavior, and product performance directly from the company's SQL database.

## Sample_Queries

Q1). Show distrinct product codes that were sold in chennai 

➡️ select distinct product_code from transactions where market_code='Mark001';

![Screenshot 2024-03-08 005942](https://github.com/Chandan65171/Sales_analysis/assets/145855999/59bc4da9-690b-4838-8890-c446ff75527f)


Q2). Show transactions where currency is US dollars  

➡️ select * from transactions where currency='USD';

![Screenshot 2024-03-08 010147](https://github.com/Chandan65171/Sales_analysis/assets/145855999/ea5de60f-7035-4d8b-bf48-263fb23ce634)

Q3). Show transactions in 2020 join by date table 

➡️ select t.* , d.* from transactions as t join date as d on d.date=t.order_date where year=2020;

![Screenshot 2024-03-08 010222](https://github.com/Chandan65171/Sales_analysis/assets/145855999/9c23ea8c-9eb8-41a7-90cc-65f4a1b73c64)

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
        
![Screenshot 2024-03-08 010318](https://github.com/Chandan65171/Sales_analysis/assets/145855999/890cbfc9-6ba1-4b35-a7b4-93da3c0d6c43)

  ➡️ etc.
        
Executed all SQL queries using a preferred SQL client or command line.

 ## Aim
 ➡️ This project aims to provide insights into:
 
 💠 Sales performance: Overall sales trends, top-performing products and regions.
 
 💠 Customer behavior: Identify buying patterns and key customer segments.
 
 💠 Market analysis: Understand market trends and competitor performance.
 
 💠 Improve sales strategies and identify new growth opportunities.
 
 💠 Optimize product offerings and marketing campaigns.
 
 💠 Make data-driven decisions for better resource allocation.

##  Tools used
 💠 SQL (Query Language)
 
 💠 MySQL (Database) 
