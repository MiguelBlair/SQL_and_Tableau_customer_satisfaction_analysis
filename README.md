# Customer Satisfaction Analysis

## Project Overview
This project focuses on customer segmentation for supermarkets, a dynamic sector. We gain insights into how different groups influence sales and profitability by analyzing customer demographics and purchasing behaviors. This analysis is valuable for refining marketing strategies and enhancing customer engagement, specifically for supermarkets aiming to optimize operations.

## Data Collection
- Data set Source: [Aung Pyae](https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales) (CSV format).
- Tools Used: Tableau for visualization and MySQL with VS code for querying the data, cleaning, and extraction.

### Initial Data Import & Preview
The dataset was imported into a MySQL schema using the load-in file query. Queries were then run to preview the data and identify key insights and necessary cleaning steps.

```python
# Load pandas library
import pandas as pd

# Read the data
df = pd.read_csv('data_set/supermarket_sales.csv')

# Preview the data
df
```

The dataset contains 1,000 rows and 17 columns. Key columns include: `Invoice_ID`, `Branch`, `City`, `Customer_type`, `Gender`, `Product_line`, `Total`, `Date`, `Payment`, `gross_income`, and `Rating`.

### Data Cleaning
- **Duplicate check:** No duplicate rows found.
- **Null value check:** No null values found.
- **Safe Table:** Created a safe copy of the table containing only relevant columns for analysis.

Most data types were correctly set to ensure accurate analysis and visualization.

## Data Analysis Goals
1. **Sales Trends by Product Line:** Aggregate total sales over time.
2. **Average Purchase by Customer Type & Gender:** Compute average transaction values and frequency.
3. **Highest Profit Margins by Product Line & Branch:** Identify the most profitable product lines and branches.
4. **Impact of Payment Method on Transaction Value:** Compare average transaction values across payment methods.

## Key Insights

### 1. Sales Trends by Product Line
Top performers:
- **Sports and Travel** had consistently high sales, peaking in January 2019.
- **Home and Lifestyle** saw the highest sales in March.

Other trends:
- **Health and Beauty** experienced fluctuations.
- **Electronic Accessories** peaked in January but declined by March.

Visualization: [Sales Trends over time](https://public.tableau.com/shared/BJQCPTJ9P?:display_count=n&:origin=viz_share_link)

### 2. Highest-Rated Product Categories
- **Food and Beverages** received the highest average rating (7.11).
- **Fashion Accessories** (7.03) and **Health and Beauty** (7.00) also scored well.

Visualization: [Top-Rated Products](https://public.tableau.com/shared/SY4DCX9FB?:display_count=n&:origin=viz_share_link)

### 3. Profit Margins by Product Line & Branch
All product lines and branches had a consistent profit margin of 4.76%, indicating a standardized pricing structure.

Visualization: [Profit Margins](https://public.tableau.com/views/SQLandTableauCustomersatisfactionanalysis/Story1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

### 4. Impact of Payment Method on Transaction Value
- **Cash** had the highest average transaction value (₹326.18).
- **Credit Card**: ₹324.01.
- **Ewallet**: ₹318.82.

Visualization: [Payment Method Impact](https://public.tableau.com/shared/N42BZPKS2?:display_count=n&:origin=viz_share_link)

## Summary
This analysis provides key insights into sales trends, customer satisfaction, profit margins, and payment methods. It highlights opportunities to focus on high-performing product lines, improve profitability, and understand customer behaviors based on payment preferences.

Thank you for reviewing this project. Feel free to provide any feedback or suggestions!
