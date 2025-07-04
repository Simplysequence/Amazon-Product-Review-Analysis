# Amazon-Product-Review-Analysis

### Table of Content
-    [Project Preview](#Project-preview)
-    [Data Sources](#Data-sources)
-    [Tools Used](#Tools-Used)
-    [Data Cleaning and Preparation](#Data-Cleaning-and-Preparation)
-    [Exploratory Data Analysis](#Exploratory-data-analysis)
-    [Data Analysis](#Data-analysis)

### Project Overview
---
The goal of this data analysis project is to produce insights that can direct marketing tactics, consumer interaction, and product enhancement. I aim to have sufficient understanding to make rational decisions by analyzing the various parameters in the data that has been received.

### Data Sources
---
The primary source of data used here contains information scraped from Amazon product pages

### Tools Used
---
-  Microsoft Excel [Download Here](https://www.microsoft.com)
    1. For Data Cleaning
    2. For Analysis with Pivot Tables
    3. For Visualization using Charts
  
### Data Cleaning and Preparation
---
In the initial phase of Data Cleaning and Preparation, we perform the following actions
-    Data Loading and Inspection
-    Data Cleaning and Formatting (Duplicates removed, categories standardized)
-    Included additional columns needed for more analysis (Price_Bucket, Discount_Interval, Potential_Revenue,Ratingg Bin)

### Exploratory Data Analysis (EDA)
---
Below is a summary of the analysis for the 14 tasks given. Each task’s methodology and output are condensed for clarity, with their individual pivot tables;
 
  1. Average Discount Percentage by Category
     - Method: Pivot table grouping by category, averaging discount_percentage.
     - Excel Pivot: Rows = category, Values = discount_percentage (Average).
     - Output:
  
  2. Number of Products per Category
     - Method: Count unique product_name per category using a pivot table.
     - Excel Pivot: Rows = category, Values = product_name (Count).
     - Output:

  3. Total Number of Reviews per Category
     - Method: Sum rating_count per category.
     - Excel Pivot: Rows = category, Values = rating_count (Sum).
     - Output:
    
  4. Products with Highest Average Ratings
     - Method: Sort by rating (descending), filter for rating_count ≥ 50.
     - Excel: Sort rating column, filter rating_count ≥ 50, display top 10.
     - Output:

  5. Average Actual vs. Discounted Price by Category
     - Method: Pivot table averaging actual_price and discounted_price by category.
     - Excel Pivot: Rows = category, Values = actual_price (Average), discounted_price (Average).
     - Output:

  6. Products with Highest Number of Reviews
     - Method: Sort by rating_count (descending), display top 10.
     - Excel:Sort rating_count column, display top 10 with product_name, category, rating_count.
     - Output:

  7. Number of Products with Discount ≥50%
     - Method: Filter discount_percentage ≥ 50, count rows.
     - Excel Filter: discount_percentage ≥ 50, count rows.
     - Output

  8. Distribution of Product Ratings
     - Method: Rating bin, count products per bin.
     - Excel Pivot: Rows = Rating bin, Values = product_name (Count).
     - Output:

  9. Total Potential Revenue by Category
     - Method: Calculate potential_revenue = actual_price * rating_count, sum by category.
     - Excel Pivot: Rows = category, Values = potential_revenue (Sum).
     - Output:

 10. Number of Unique Products per Price Range Bucket
     - Method: Bin actual_price into <₹200, ₹200–₹500, >₹500, count unique product_name.
     - Excel Pivot: Rows = Price_Bucket, Values = product_name (Count).
     - Output:

 11. Rating vs. Discount Level
     - Method: Bin discount_percentage into 0–10%, 10–20%, etc., calculate average rating.
     - Excel Pivot: Rows = Discount_Interval, Values = rating (Average), product_name (Count).
     - Output:

 12. Products with <1,000 Reviews
     - Method: Filter rating_count < 1,000, count rows.
     - Output:

 13. Categories with Highest Discounts
     - Method: Pivot table with max discount_percentage per category.
     - Excel Pivot: Rows = category, Values = discount_percentage (Max).
     
     

### Data Analysis
---
This is where we include some basic llines of codes or Queries or even some of the DAX expressions used during your analysis;

```  SQL
Select * From A, B, C
Where A> 15
```
### Results/Findings


### Recommendations


### Data Visualization

![REGION CHART](https://github.com/user-attachments/assets/ae0c8ea2-61f3-4f4d-99c3-1bbf4c298454)


![TOP 10 REVENUE CHART](https://github.com/user-attachments/assets/3b7434a5-b9db-401d-bf3e-0f6e5b5ac9b6)

