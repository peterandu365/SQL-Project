# E-Commerce Data Analysis using SQL

## Project/Goals
My project goal is to:

    - polish the SQL language skills;
    - run my first ETL workflow;
    - get familiar with the pgAdmin 4 environments;
    - master the MD file writing skills;
    - practice the git commands to submit versions.

## Process

1. Import CSV format data into pgAdmin 4 by using the query command line.
2. Drop the empty column.
3. Delete duplicated entries from table ***analytics***.
4. Fix the product_category values.
5. Fix the price/revenue values by dividing by 1,000,000.
6. Resolving questions by querying.
7. Quality Assurance.
8. Documenting.
9. Submitting.

## Results

This data is about an e-commerce website's product sales, transactions and product inventory. The all_sessions table is used to answer most of the questions. 

By calculating the sum or average of the numerical variables, such as transaction or number of ordered products, I can answer question 1 and question 2.

Grouping by country and city and counting on the nominal categorical values, such as the product SKU, name or categories, I can get the rank or overall score for the popularity of the products/categories over the country/city, which can be used to answer questions 3 & 4. Adding a ***cume_dist()*** window function can help find out the statistical ranking across PARTITIONs.

Two answer question 5, I need to apply the correlation function to numerical variables. The correlation can be calculated between two numerical columns in the table all_sessions, to confirm the existing relationship between the most profitable products (product generates the most revenue) and the website usage. The correlation can also be calculated between two tables, by inner joining them on the product SKU. It can be concluded that one of the impacts of revenue generated from popular products is to encourage the owner to increase the stock for those products.

## Challenges 

1. How to import CSV by command line?
2. Getting familiar with pgAdmin.
3. How to back up and duplicate tables?
4. Assigning Primary Key and Foreign Key after the data is imported to the pgAdmin database.
5. Is the Primary Key and Foreign Key mandatory for generating an ERD chart?
6. How to find and drop all the empty columns in a database by automation?
7. How to fill a continuous sequence of natural numbers for a newly created column？
8. Why pgAdmin can not create a column with a Time datatype?
9. How to enable Grammarly in Visual Studio Code?
10. How to examine the largest length across all the values in a specific column?
11. How to use regular expressions together with ProgreSQL?
12. Why the round() function does not work with a decimal setting?
13. What are potential patterns when analyzing data?


## Future Goals

1. Master regular expression;
2. Improve proficiency.
3. Optimizing SQL coding by using a temporary table.


