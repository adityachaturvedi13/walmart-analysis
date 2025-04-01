# Walmart Sales Data Analysis - SQL Project

## About

This project is a personal initiative to analyze Walmart's sales data using SQL. The goal was to extract meaningful insights into branch and product performance, sales patterns, and customer behavior, ultimately to inform potential sales strategy improvements.

## Project Objectives

The primary objective was to leverage SQL to explore and understand Walmart's sales data, focusing on identifying key factors that influence sales across different branches. This was an exercise in applying SQL skills to a real-world dataset.

## Data Source

The dataset used for this project was obtained from the Kaggle Walmart Sales Forecasting Competition. It includes sales transactions from three Walmart branches: Mandalay, Yangon, and Naypyitaw. 

## Data Description

The dataset comprises 17 columns and 1000 rows. Here's a breakdown of the columns and their data types:

| Column             | Description                                    | Data Type        |
|--------------------|------------------------------------------------|------------------|
| `invoice_id`       | Invoice of the sales made                      | VARCHAR(30)      |
| `branch`           | Branch at which sales were made                | VARCHAR(5)       |
| `city`               | The location of the branch                     | VARCHAR(30)      |
| `customer_type`    | The type of the customer                        | VARCHAR(30)      |
| `gender`           | Gender of the customer making purchase         | VARCHAR(10)      |
| `product_line`     | Product line of the product sold                | VARCHAR(100)     |
| `unit_price`       | The price of each product                      | DECIMAL(10, 2)   |
| `quantity`         | The amount of the product sold                  | INT              |
| `VAT`              | The amount of tax on the purchase              | FLOAT(6, 4)      |
| `total`            | The total cost of the purchase                 | DECIMAL(12, 4)   |
| `date`             | The date on which the purchase was made        | DATETIME         |
| `time`             | The time at which the purchase was made        | TIME             |
| `payment`          | The total amount paid                          | DECIMAL(10, 2)   |
| `cogs`             | Cost Of Goods Sold                             | DECIMAL(10, 2)   |
| `gross_margin_pct` | Gross margin percentage                        | FLOAT(11, 9)     |
| `gross_income`     | Gross Income                                   | DECIMAL(12, 4)   |
| `rating`           | Rating                                         | FLOAT(2, 1)      |

## Analysis Areas

In this project, I focused on using SQL to explore three key areas:

1.  **Product Analysis:** Analyzing product lines to identify top performers and areas for potential improvement. 
   
2.  **Sales Analysis:** Investigating sales trends to evaluate the effectiveness of sales strategies. 
   
3.  **Customer Analysis:** Segmenting customers, understanding their purchasing behavior, and assessing profitability. 

## SQL Methodology

The project was structured using the following SQL-driven approach:

1.  **Data Wrangling:**
   
   * Examined the data for NULL values. In this dataset, the tables were designed with "NOT NULL" constraints, so no specific NULL value handling was required. 
   
2.  **Feature Engineering (using SQL):**
   
   * Created new columns using SQL queries to derive additional insights:
        * `time_of_day` (Morning, Afternoon, Evening) to analyze sales by time of day. 
        * `day_name` (e.g., Mon, Tue, Wed) to analyze sales by day of the week. 
        * `month_name` (e.g., Jan, Feb, Mar) to analyze sales by month. 
   
3.  **Exploratory Data Analysis (EDA) with SQL:**
   
   * Conducted EDA by formulating and executing SQL queries to answer specific business questions. 

## Business Questions (SQL Queries)

The following questions were addressed using SQL queries:

### Generic Questions

1.  How many distinct cities are in the dataset? 
   
2.  Which city is each branch located in? 

### Product Analysis

1.  How many distinct product lines are in the dataset? 
   
2.  What is the most common payment method? 
   
3.  What is the most selling product line? 
   
4.  What is the total revenue by month? 
   
5.  Which month recorded the highest Cost of Goods Sold (COGS)? 
   
6.  Which product line generated the highest revenue? 
   
7.  Which city has the highest revenue? 
   
8.  Which product line incurred the highest VAT? 
   
9.  For each product line, create a `product_category` column (using SQL CASE statements) indicating "Good" or "Bad" based on sales relative to the average. 
   
10. Which branch sold more products than the average product sold? 
   
11. What is the most common product line by gender? 
   
12. What is the average rating of each product line? 

### Sales Analysis

1.  What is the number of sales made in each time of day per weekday? ]
   
2.  Which customer type generates the highest revenue? 
   
3.  Which city has the largest tax percent/VAT? 
   
4.  Which customer type pays the most VAT? 

### Customer Analysis

1.  How many unique customer types are in the data? 
   
2.  How many unique payment methods are in the data? 
   
3.  What is the most common customer type? 
   
4.  Which customer type buys the most? 
   
5.  What is the gender of most of the customers? 
   
6.  What is the gender distribution per branch? 
   
7.  Which time of the day do customers give the most ratings? 
   
8.  Which time of the day do customers give the most ratings per branch? 
   
9.  Which day of the week has the best average ratings? 
   
10. Which day of the week has the best average ratings per branch? 

