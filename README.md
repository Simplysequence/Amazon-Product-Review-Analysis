# Amazon-Product-Review-Analysis

This is a repository where i carried out my first project while studying at The Incubator Hub. My team was tasked with analysing product and customer review data and give insights that can guide product improvement, marketing strategies and customer engagement

---
### Table of Content
-    [Project Preview](#Project-preview)
-    [Data Sources](#Data-sources)
-    [Tools Used](#Tools-Used)
-    [Data Cleaning and Preparation](#Data-Cleaning-and-Preparation)
-    [Exploratory Data Analysis](#Exploratory-data-analysis)
-    [Results/Findings](#Results/Findings)
-    [Recommendations](#Recommendations)
-    [Data Visualization](#Data-Visualization)

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

Insights: The average discount percentage varies significantly across product categories. "Homeimprovement" products lead with the highest average discount (58%), followed closely by "Computers & Accessories" (53%), "Health & Personalcare" (53%), and "Electronics" (50%). This suggests aggressive pricing strategies or competitive markets within these categories. In contrast, "Toys & Games" are listed with no average discount (0.00%), and "Officeproducts" have a very low average discount (12%). This could indicate stronger pricing power, lower competitive pressure, or a different sales strategy for these categories. Sellers might be using discounts strategically to move inventory or attract customers in specific high-discount categories.

    2. Number of Products per Category
     - Method: Count unique product_name per category using a pivot table.
     - Excel Pivot: Rows = category, Values = product_name (Count).
     - Output:

![Task 2](https://github.com/user-attachments/assets/50ba7241-8fd5-419c-b856-730fb3df4ab3)

Insights: The product listing count varies dramatically across categories. "Electronics" dominates with 490 products, followed by "Home & Kitchen" with 447 products. These two categories represent the vast majority of products in the dataset, indicating they are core offerings for sellers. Conversely, several categories like "Car & Motorbike," "Health & Personalcare," "Toys & Games," and "Musicalinstruments" have only 1 or 2 products listed. This could suggest either niche offerings, unexploited market potential, or potentially incomplete data for these categories. "Officeproducts" has a moderate presence with 31 products. This distribution highlights Amazon's current focus areas and potential gaps in product diversification.

    3. Total Number of Reviews per Category
     - Method: Sum rating_count per category.
     - Excel Pivot: Rows = category, Values = rating_count (Sum).
     - Output:

![Task 3](https://github.com/user-attachments/assets/6916b000-6060-48b1-bf69-74623b3c926f)

Insights: The total number of reviews per category dramatically highlights customer engagement levels. "Electronics" absolutely dominates with over 14.2 million reviews, reinforcing its position as the most popular and actively reviewed product category. "Home & Kitchen" follows as a distant second with nearly 3 million reviews. Categories like "Car & Motorbike," "Health & Personalcare," and "Toys & Games" have very low review counts, which correlates with their low product counts (as seen in Question 2 above). This indicates either very low customer engagement, niche products with limited reach, or possibly less popular items within those categories. The high review volume in "Electronics" suggests a highly active customer base and strong product visibility within that segment, offering valuable feedback for product improvement and marketing strategies.

    4. Products with Highest Average Ratings
     - Method: Sort by rating (descending), filter for rating_count ≥ 50.
     - Excel: Sort rating column, filter rating_count ≥ 50, display top 10.
     - Output:

![Task 4](https://github.com/user-attachments/assets/ff5789e3-78e1-42c0-8144-e66e17087436)

Insights: Several products stand out with exceptionally high average ratings. "Office Products", "Toys & Games", and "Home Improvement" achieved the highest average rating of 4.3 each. Close behind were "Computer & Accessories," with an average rating of 4.2. This indicates strong customer satisfaction and positive product experiences for these specific items. These highly-rated products represent a significant asset for Amazons clients. Further analysis into what makes these products so successful (e.g., specific features, unique selling propositions, effective marketing, quality of customer support) could provide valuable lessons to apply to other products or categories, potentially improving overall ratings and customer loyalty.

    5. Average Actual vs. Discounted Price by Category
     - Method: Pivot table averaging actual_price and discounted_price by category.
     - Excel Pivot: Rows = category, Values = actual_price (Average), discounted_price (Average).
     - Output:

![Task 5](https://github.com/user-attachments/assets/0aa86135-1e14-4622-a019-23c8963cab72)

Insights: This analysis reveals the significant impact of discounts on potential revenue across categories. Overall, the average actual price of products is 5,593, but after discounts, the average discounted price drops to 3,306, representing a substantial reduction in potential revenue.

"Electronics" shows the largest absolute difference between actual and discounted prices (approx. 10,000), reflecting its high volume and significant average discount (as seen in Question 1 above). "Home & Kitchen" also has a large difference (approx. 4,000). This indicates that while discounts in these categories are effective in driving sales, they also significantly impact the immediate revenue intake.

Categories like "Toys & Games" show no difference, as they have 150 average discount, and "Officeproducts" show a minimal difference, aligning with their low discount percentages. Sellers need to balance the attraction of discounts with their impact on overall profitability, especially in high-volume, heavily discounted categories.

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

![Task 14](https://github.com/user-attachments/assets/72bb5091-3a0f-4113-b405-4daef23d95a3)

---
### Results/Findings

1. The data reveals a varied discount strategy across product categories, with an overall average of 47%. Categories like Home improvements and Computers & Accessories show aggressive discounting, while Toys & Games and Office products exhibit minimal to no discounts.

2. The analysis indicates a significant imbalance in product distribution across categories, with Electronics having the bulk of the 1,350 product inventory. Conversely, categories such as Health & Personal Care and Toys & Games exhibit notably low product counts.

3. The data reveals a skewed distribution of reviews with Electronics driving the majority of customer feedback

4. 
---

### Recommendations


### Data Visualization

