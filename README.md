# __Apple-Retail-Sales-Analysis__

Advanced SQL Analysis of Apple Retail Sales Data
This project demonstrates advanced SQL querying techniques on a dataset of over 1 million rows from Apple retail sales.
It showcases a wide range of analytical skills, including optimizing query performance, solving real-world business 
problems, and extracting actionable insights from large datasets.
Table of Contents
1.	Project Overview
2.	Database Schema
3.	Skills Highlighted
4.	Key Business Questions Solved
5.	Performance Optimization
________________________________________
Project Overview
This project is designed to analyze Apple retail sales data, providing insights into store performance, product trends, 
and warranty claims. By leveraging advanced SQL features, the project addresses real-world business challenges and 
showcases efficient data processing techniques.
________________________________________
Database Schema
The database consists of five main tables:
•	stores: Information about Apple retail stores (e.g., store ID, name, city, country).
•	category: Product categories (e.g., category ID, category name).
•	products: Details about Apple products (e.g., product ID, name, launch date, price).
•	sales: Sales transactions (e.g., sale date, store ID, product ID, quantity).
•	warranty: Warranty claims (e.g., claim date, repair status).
Refer to the schema.sql file for detailed table definitions.
________________________________________
Skills Highlighted
•	Performance Optimization: Created indexes to enhance query execution speeds significantly.
•	Window Functions: Used for running totals, ranking, and growth analysis.
•	Complex Joins and Aggregations: Combined data from multiple tables to derive meaningful insights.
•	Data Segmentation: Analyzed trends across various timeframes and regions.
•	Correlation Analysis: Explored relationships between variables like product price and warranty claims.
________________________________________
Key Business Questions Solved
1.	How many stores exist in each country?
2.	Which store sold the highest number of units in the past year?
3.	What is the average price of products in each category?
4.	What percentage of warranty claims were rejected?
5.	Which store had the highest percentage of completed warranty claims?
6.	What is the least-selling product in each country for each year?
7.	How many warranty claims were filed within 180 days of purchase?
8.	What is the year-over-year growth ratio for each store?
9.	What is the monthly running total of sales for each store over the past four years?
For the complete list of queries and results, check the queries.sql file.
________________________________________
Performance Optimization
Before optimization:
•	Query execution time: 136.423 ms
After creating indexes:
•	Query execution time: 6.324 ms
Indexes created:
•	sales_product_id on sales(product_id)
•	sales_store_id on sales(store_id)
•	sales_quantity on sales(quantity)
•	sale_date on sales(sale_date)
•	sales_product_id_store_id on sales(product_id, store_id)

Explaination

This project was all about analyzing Apple retail sales data with over 1 million rows.
The dataset included detailed information about products, sales transactions, stores, and
warranty claims from various Apple retail locations worldwide. The goal was to solve real-world
business problems using advanced SQL techniques.

I started by exploring the data to understand the schema. There were five main tables: stores,
sales, products, category, and warranty. Each table contributed unique data dimensions, like
store locations, product details, and sales trends.

I worked on solving key business problems like identifying the total sales for each store, finding
the best-selling products, analyzing warranty claim trends, and even determining year-over-year growth
for stores. For example, I calculated the percentage of warranty claims rejected and identified stores
with the highest sales in the last year.

I also implemented advanced SQL techniques like window functions for ranking and running totals, indexing
to optimize query performance, and correlation analysis to see relationships between product price and warranty claims.

One interesting part of the project was optimizing query performance. Initially, a query on the sales table
took over 136 ms to execute. After creating indexes on key columns like product_id and store_id, the execution time dropped to just 6 ms.

Overall, this project helped me build a strong understanding of handling large datasets, optimizing SQL queries, 
and deriving actionable insights. It’s a great example of how I can use data to answer real-world business questions."
