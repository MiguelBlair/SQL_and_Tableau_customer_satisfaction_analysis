# Customer Satisfaction & Segmentation Analysis

## Project Overview
This project focuses on customer segmentation for supermarkets, a dynamic sector. By analyzing customer demographics and purchasing behaviors, we gain insights into how different groups influence sales and profitability. This analysis is valuable for refining marketing strategies and enhancing customer engagement, specifically for supermarkets aiming to optimize operations.

## Data Collection
- Dataset Source: [Aung Pyae](https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales) (CSV format).
- Tools Used: Tableau for visualization and SQL Server Management Studio (SSMS) for data querying, cleaning, and extraction.

### Initial Data Import & Preview
The dataset was imported into a SQL Server schema using the data import wizard. Queries were then run to preview the data and identify key insights and necessary cleaning steps.

```python
# Load pandas library
import pandas as pd

# Read the data
df = pd.read_csv('Assets/supermarket_sales.csv')

# Preview the data
df
```

The dataset contains 1,000 rows and 17 columns. Key columns include: `Invoice_ID`, `Branch`, `City`, `Customer_type`, `Gender`, `Product_line`, `Total`, `Date`, `Payment`, `gross_income`, and `Rating`.

### Data Cleaning
- **Duplicate check:** No duplicate rows found.
- **Null value check:** No null values found.
- **Staging Table:** Created a staging copy of the table containing only relevant columns for analysis.

Data types were correctly set to ensure accurate analysis and visualization.

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

Visualization: [Sales Trends Tableau](https://public.tableau.com/shared/6B5GY3X4T)

### 2. Highest-Rated Product Categories
- **Food and Beverages** received the highest average rating (7.11).
- **Fashion Accessories** (7.03) and **Health and Beauty** (7.00) also scored well.

Visualization: [Top-Rated Products Tableau](https://public.tableau.com/shared/NFMMNT5B2)

### 3. Profit Margins by Product Line & Branch
All product lines and branches had a consistent profit margin of 4.76%, indicating a standardized pricing structure.

Visualization: [Profit Margins Tableau](https://public.tableau.com/views/CustomersatisfactionSQLandTableauanalysis/Story1)

### 4. Impact of Payment Method on Transaction Value
- **Cash** had the highest average transaction value (₹326.18).
- **Credit Card**: ₹324.01.
- **Ewallet**: ₹318.82.

Visualization: [Payment Method Impact Tableau](https://public.tableau.com/shared/5WZFGNZ47)

## Summary
This analysis provides key insights into sales trends, customer satisfaction, profit margins, and payment methods. It highlights opportunities to focus on high-performing product lines, improve profitability, and understand customer behaviors based on payment preferences.

Thank you for reviewing this project. Feel free to provide any feedback or suggestions!
