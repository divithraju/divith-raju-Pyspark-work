# Project: PySpark Data Processing Toolkit
This repository contains a collection of PySpark scripts designed to handle various data processing and analysis tasks. These scripts cover topics like sequential numbering, first purchase date determination, data reshaping, rolling averages, missing value detection, handling mixed delimiters, and missing data imputation. Each script is a standalone solution, demonstrating how PySpark can be used to solve practical data engineering problems.

# Contents
1.Sequential Numbering by Group: Generates a sequential number for each row within each group, ordered by date.

2.First Purchase Date Calculation: Determines the first purchase date for each user from a dataset of purchase records.

3.Pivoting Sales Data: Reshapes sales data to create a long format for easier analysis.

4.7-Day Rolling Average Calculation: Calculates a 7-day rolling average of sales quantities for each product.

5.Finding Missing Numbers in a Sequence: Detects missing numbers in a sequence, useful for identifying gaps in data.

6.Handling Mixed Delimiters: Processes data with mixed delimiters in a single row using custom logic in PySpark.

7.Imputing Missing Sales Amounts: Replaces missing values in the sales amount column with the average sales amount.

# Detailed Descriptions
1.Sequential Numbering by Group: Uses the row_number() function within a window specification to generate sequential numbers for each row in a group, ordered by date. This is useful for scenarios like ranking or assigning unique IDs within grouped data.

2.First Purchase Date Calculation: Aggregates user purchase data to find the earliest purchase date for each user, demonstrating how to group and summarize data.

3.Pivoting Sales Data: Transforms sales data from wide format (multiple columns for each month) to a long format, making it easier to analyze monthly trends.

4.7-Day Rolling Average Calculation: Demonstrates how to calculate rolling averages over a window of time for each product, which is essential for time-series analysis.

5.Finding Missing Numbers in a Sequence: Identifies gaps in a numeric sequence, helping to detect missing records in a dataset.

6.Handling Mixed Delimiters: Shows how to split and process data with multiple delimiters in the same row, which is common in messy or inconsistent datasets.

7.Imputing Missing Sales Amounts: Demonstrates how to handle missing values by calculating the average and using it to replace None values, ensuring data completeness.

# How to Use Each Script
1.Sequential Numbering by Group (sequentail.py): Run the script to generate sequential numbers for rows within grouped data.

2.First Purchase Date Calculation (purchase.py): Run this script to calculate the first purchase date for each user in your dataset.
Pivoting Sales Data (pivot.py): Use this script to convert wide sales data into a long format, creating one row per product-month combination.

3.7-Day Rolling Average Calculation (moving-avg.py): Calculate a rolling average for sales quantities over a 7-day window.

4.Finding Missing Numbers (missing.py): Detect missing numbers in a sequence, helping to identify gaps in numeric data.

5.Handling Mixed Delimiters (delimiter.py): Split and process rows with mixed delimiters using custom logic.

6.Imputing Missing Sales Amounts (avg-sales-amount.py): Replace missing values in sales data with the average amount, ensuring data consistency.
# License
This project is licensed under the MIT License.


