# Walmart Sales Analysis

A comprehensive SQL analysis of Walmart sales data to understand product performance, customer behavior, and revenue patterns across multiple branches.

## Project Overview

This project performs exploratory data analysis on Walmart sales transactions using MySQL to uncover insights about product lines, customer segments, and sales trends. The analysis includes feature engineering to create time-based segments and extensive queries to answer key business questions.

## Dataset

- **Source**: Walmart sales transaction records
- **Database**: MySQL
- **Key Fields**: invoice_id, branch, city, customer_type, gender, product_line, unit_price, quantity, VAT, total, date, time, payment_method, cogs, rating
- **Product Lines**: Electronic accessories, Fashion accessories, Food and beverages, Health and beauty, Home and lifestyle, Sports and travel

## Feature Engineering

Created three new time-based features to enable temporal analysis:

1. **time_of_day**: Categorized transactions into Morning, Afternoon, and Evening
2. **day_name**: Extracted day of the week from transaction dates
3. **month_name**: Extracted month from transaction dates

## Analysis Categories

### Product Analysis
- Identified product line distribution and best-selling categories
- **Top performer**: Electronic accessories had the highest total sales
- Analyzed revenue and COGS (Cost of Goods Sold) by product line
- Calculated VAT distribution across product lines
- Classified product lines as "Good" or "Bad" performers based on average sales
- Examined gender preferences for different product lines
- Evaluated average customer ratings per product line

### Sales Analysis
- Tracked sales volume by time of day and weekday
- Analyzed revenue distribution by customer type (Member vs. Normal)
- Examined payment method preferences (Cash was most common)
- Calculated revenue and VAT patterns across cities and branches
- Identified branches exceeding average product sales

### Customer Analysis
- Segmented customers by type and analyzed purchasing patterns
- Examined gender distribution overall and by branch
- Analyzed rating patterns by time of day and branch
- Identified peak rating times for each branch
- Calculated average ratings by day of week

## Key Findings

- **Payment Preference**: Cash was the most frequently used payment method
- **Best-Selling Category**: Electronic accessories generated the highest sales volume
- **Branch Performance**: Identified which branches sold more products than average
- **Customer Behavior**: Members and normal customers showed different purchasing patterns
- **Temporal Trends**: Sales and ratings varied by time of day and day of week

## Technical Skills Demonstrated

- Feature engineering with date/time functions (DAYNAME, MONTHNAME)
- Complex SQL queries with GROUP BY, HAVING, and subqueries
- Conditional logic using CASE statements
- Window functions and aggregations
- Database schema modification (ALTER TABLE, UPDATE)
- Comparative analysis using nested queries

## Tools & Technologies

- **Database**: MySQL
- **Language**: SQL
- **Key Techniques**: Feature engineering, aggregation, conditional logic, data segmentation

## Business Applications

This analysis provides insights for:
- Inventory optimization based on product line performance
- Staffing decisions based on peak sales times
- Targeted marketing campaigns by customer segment
- Branch-level performance improvement strategies
- Payment processing infrastructure planning

## Repository Structure

```
walmart_sales_analysis/
├── README.md
└── walmart_sales_analysis.sql
```

## How to Use

1. Import the Walmart sales dataset into MySQL
2. Run the feature engineering queries to add time-based columns
3. Execute analysis queries to generate insights

## Author

Mark Isabelle  
[LinkedIn](https://linkedin.com/in/mark-isabelle-a113b8325) | [GitHub](https://github.com/markisabelle)
