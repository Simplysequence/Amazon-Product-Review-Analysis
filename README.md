# Amazon-Product-Review-Analysis

This is where i carried out my first project while studying at The Incubator Hub. I studied the raw data, cleaned it up and analyzed using charts and tables

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

### Exploratory Data Analysis
---
Below is a summary of the analysis for the 14 tasks given. Each task’s methodology and output are condensed for clarity, with their individual pivot tables;
 
  1. Average Discount Percentage by Category
     - Method: Pivot table grouping by category, averaging discount_percentage.
     - Excel Pivot: Rows = category, Values = discount_percentage (Average).
     - Output:

![Task 1](https://github.com/user-attachments/assets/646e6d54-4a3a-4fcc-a0db-6ee2999ae134)

  2. Number of Products per Category
     - Method: Count unique product_name per category using a pivot table.
     - Excel Pivot: Rows = category, Values = product_name (Count).
     - Output:

![Task 2](https://github.com/user-attachments/assets/50ba7241-8fd5-419c-b856-730fb3df4ab3)

  3. Total Number of Reviews per Category
     - Method: Sum rating_count per category.
     - Excel Pivot: Rows = category, Values = rating_count (Sum).
     - Output:

![Task 3](https://github.com/user-attachments/assets/6916b000-6060-48b1-bf69-74623b3c926f)

  4. Products with Highest Average Ratings
     - Method: Sort by rating (descending), filter for rating_count ≥ 50.
     - Excel: Sort rating column, filter rating_count ≥ 50, display top 10.
     - Output:

![Task 4](https://github.com/user-attachments/assets/ff5789e3-78e1-42c0-8144-e66e17087436)

  5. Average Actual vs. Discounted Price by Category
     - Method: Pivot table averaging actual_price and discounted_price by category.
     - Excel Pivot: Rows = category, Values = actual_price (Average), discounted_price (Average).
     - Output:

![Task 5](https://github.com/user-attachments/assets/0aa86135-1e14-4622-a019-23c8963cab72)

  6. Products with Highest Number of Reviews
     - Method: Sort by rating_count (descending), display top 10.
     - Excel:Sort rating_count column, display top 10 with product_name, category, rating_count.
     - Output:

![Task 6](https://github.com/user-attachments/assets/3b73f399-7e86-4cee-9543-cd6b1f5fe573)

  7. Number of Products with Discount ≥50%
     - Method: Filter discount_percentage ≥ 50, count rows.
     - Excel Filter: discount_percentage ≥ 50, count rows.
     - Output

![Task 7](https://github.com/user-attachments/assets/923744fc-ce91-4213-b403-aa95fbc2595c)

  8. Distribution of Product Ratings
     - Method: Rating bin, count products per bin.
     - Excel Pivot: Rows = Rating bin, Values = product_name (Count).
     - Output:

![Task 8](https://github.com/user-attachments/assets/f21da3f9-c062-4c3d-8e62-17b5a502ac52)

  9. Total Potential Revenue by Category
     - Method: Calculate potential_revenue = actual_price * rating_count, sum by category.
     - Excel Pivot: Rows = category, Values = potential_revenue (Sum).
     - Output:

![Task 9](https://github.com/user-attachments/assets/4d7d1b85-1368-4355-9924-0b95d8312fe2)

 10. Number of Unique Products per Price Range Bucket
     - Method: Bin actual_price into <₹200, ₹200–₹500, >₹500, count unique product_name.
     - Excel Pivot: Rows = Price_Bucket, Values = product_name (Count).
     - Output:

![Task 10](https://github.com/user-attachments/assets/94d97aab-d55a-4739-9484-2c17e2d73728)

 11. Rating vs. Discount Level
     - Method: Bin discount_percentage into 0–10%, 10–20%, etc., calculate average rating.
     - Excel Pivot: Rows = Discount_Interval, Values = rating (Average), product_name (Count).
     - Output:

![Task 11](https://github.com/user-attachments/assets/c8a41203-21ea-4ab2-91a0-eb8f2bd2543c)

 12. Products with <1,000 Reviews
     - Method: Filter rating_count < 1,000, count rows.
     - Output:

![Task 12](https://github.com/user-attachments/assets/096ac8ac-17e6-48eb-9654-a965b6c6a708)

 13. Categories with Highest Discounts
     - Method: Pivot table with max discount_percentage per category.
     - Excel Pivot: Rows = category, Values = discount_percentage (Max).
     - Output:

![Task 13](https://github.com/user-attachments/assets/c06b075c-5d46-467a-b2fc-f95bfbc2987d)

 14. Top 5 Products by Rating and Reviews
     - Method: Calculate Composite_Score = 0.6*rating + 0.4*log(rating_count), sort top 5.
     - Excel Pivot: Rows = product_name, category, Values = Composite_Score (Average), sort top 5.
     - Output:



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

