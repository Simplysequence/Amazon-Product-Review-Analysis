# Amazon-Product-Review-Analysis

This is a repository where i carried out my first project while studying at The Incubator Hub. My team was tasked with analysing product and customer review data and give insights that can guide product improvement, marketing strategies and customer engagement

---
### Table of Content
-    [Project Preview](#Project-preview)
-    [Data Sources](#Data-sources)
-    [Tools Used](#Tools-Used)
-    [Data Cleaning and Preparation](#Data-Cleaning-and-Preparation)
-    [Exploratory Data Analysis](#Exploratory-data-analysis)
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

Insights: The analysis of review counts by product name reveals the most popular and highly engaged products. "Electronics" stands out significantly with over 14 million reviews, making it the product with the highest customer engagement. Other products with a very high number of reviews include "Computer & Accessories", "Home & Kitchen", with each exceeding 6 million and over 2 million reviews respectively.
These products are highly visible and trusted by a large customer base. For Amazon's clients, these products represent strong performers that can be leveraged in marketing campaigns, used as benchmarks for product development, or serve as anchor products to drive traffic and cross-selling opportunities. The sheer volume of reviews for these products also provides a rich source of customer feedback for product refinement and service improvement.

    7. Number of Products with Discount ≥50%
     - Method: Filter discount_percentage ≥ 50, count rows.
     - Excel Filter: discount_percentage ≥ 50, count rows.
     - Output

![Task 7](https://github.com/user-attachments/assets/923744fc-ce91-4213-b403-aa95fbc2595c)

Insights: A significant portion of products are offered with a discount of 50% or more. This indicates that nearly half of the product listings are subjected to aggressive pricing strategies. This could be a response to high market competition, an effort to clear inventory, or a deliberate strategy to attract price-sensitive customers. The relatively even split between highly discounted and less discounted products suggests a diversified pricing approach by sellers on Amazon.

    8. Distribution of Product Ratings
     - Method: Rating bin, count products per bin.
     - Excel Pivot: Rows = Rating bin, Values = product_name (Count).
     - Output:

![Task 8](https://github.com/user-attachments/assets/f21da3f9-c062-4c3d-8e62-17b5a502ac52)

Insights: The distribution of product ratings shows a strong positive skew, indicating that the majority of products have high ratings. The highest concentration of products falls within the 4.0 to 4.5 rating range, with 914 products at 4.0-4.5. This highlights generally good customer satisfaction across the listed products. As ratings decrease, the number of products also significantly drops (e.g., only 2 products at 2.0-2.5). This positive trend in ratings is a strong indicator of perceived product quality and customer loyalty for sellers on Amazon. It also suggests that products falling below the 4.0 mark might require attention for improvement.

    9. Total Potential Revenue by Category
     - Method: Calculate potential_revenue = actual_price * rating_count, sum by category.
     - Excel Pivot: Rows = category, Values = potential_revenue (Sum).
     - Output:

![Task 9](https://github.com/user-attachments/assets/4d7d1b85-1368-4355-9924-0b95d8312fe2)

Insights: The total potential revenue by category reveals immense market opportunities, particularly dominated by "Electronics" with an astounding ₹91.3 billion. This colossal figure underscores the massive scale of this category on Amazon and its potential for high sales volume, driven by both high prices and extensive customer engagement (as seen in review counts). "Computers & Accessories" follows as a distant but significant second with over ₹11.6 billion in potential revenue.
Other categories, while much smaller in comparison, still represent substantial markets (e.g., "Musicalinstruments" with ₹10.4 Billion, "Officeproducts" with ₹60 million). This analysis helps prioritize categories for investment, marketing spend, and inventory management, focusing resources on areas with the highest revenue-generating potential. The high potential in Electronics, even with significant discounting, highlights its strategic importance.

    10. Number of Unique Products per Price Range Bucket
     - Method: Bin actual_price into <₹200, ₹200–₹500, >₹500, count unique product_name.
     - Excel Pivot: Rows = Price_Bucket, Values = product_name (Count).
     - Output:

![Task 10](https://github.com/user-attachments/assets/94d97aab-d55a-4739-9484-2c17e2d73728)

Insights: The distribution of unique products across price ranges reveals a clear focus on higher-priced items. A dominant majority of products, 1165 of 1350 (approximately 86.3%), fall into the "> ₹500" price bucket. Products while in the "₹200-₹500" range are significantly fewer (151 products), and there are very few products in the "< ₹200" range (only 34 products).
This suggests that sellers on Amazon, or at least within this dataset, primarily target the mid-to-high price segments. This could be due to the nature of the dominant categories (Electronics, Home & Kitchen often feature higher-priced items) or a strategic decision to focus on higher-value products. While this indicates a strong presence in premium segments, it also suggests potential opportunities or gaps in the very budget-friendly product offerings if market demand exists there.

    11. Rating vs. Discount Level
     - Method: Bin discount_percentage into 0–10%, 10–20%, etc., calculate average rating.
     - Excel Pivot: Rows = Discount_Interval, Values = rating (Average), product_name (Count).
     - Output:

![Task 11](https://github.com/user-attachments/assets/c8a41203-21ea-4ab2-91a0-eb8f2bd2543c)

Insights: Products with a mid-range discount range (40%-50%) have the highest rating count (974). Conversely, products with the highest discount range (90%-100%) have the lowest rating count (25).
This counter-intuitive finding suggests that high-quality or highly demanded products might not require aggressive discounting to achieve excellent ratings and attract buyers. It implies that customers are willing to pay closer to the actual price for products they perceive as superior. Conversely, while deep discounts can attract buyers, they might be slightly associated with products that receive marginally mid satisfaction scores, or they are strategically used for products that need a stronger push to sell. This challenges the notion that heavily discounted items are necessarily of lower quality, but rather highlights that strong products can maintain high ratings even without significant price cuts.

    12. Products with <1,000 Reviews
     - Method: Filter rating_count < 1,000, count rows.
     - Output:

![Task 12](https://github.com/user-attachments/assets/096ac8ac-17e6-48eb-9654-a965b6c6a708)

Insights: The analysis reveals that 309 products have fewer than 1,000 reviews. This constitutes a notable portion of the total products (approximately 22.89% of the 1350 products in the analyzed dataset).
The distribution of reviews is highly polarized:
A significant number of products (1041) have over 1,000 reviews, indicating highly popular and established items with massive customer engagement.
In contrast, the 309 products with fewer than 1,000 reviews suggest they might be newer listings, niche products, or struggling to gain visibility and traction.
For Amazon's clients, these low-review products present an opportunity for targeted marketing, review generation campaigns, or re-evaluation of their product-market fit. Understanding this distribution helps in prioritizing which products need attention to boost their online presence and customer feedback.

    13. Categories with Highest Discounts
     - Method: Pivot table with max discount_percentage per category.
     - Excel Pivot: Rows = category, Values = discount_percentage (Max).
     - Output:

![Task 13](https://github.com/user-attachments/assets/c06b075c-5d46-467a-b2fc-f95bfbc2987d)

Insights: Reconfirming findings from Question 1, "Homeimprovement" (58%), "Computer Accessories" (53%), and "Health & PersonalCare" (53%) are the categories where products carry the highest average discount percentages. This indicates these are highly competitive categories where sellers frequently employ aggressive pricing strategies to attract customers or manage inventory.
For Amazon's clients, these categories represent areas where consumers expect significant price reductions. Strategic discounting is crucial here, but it also necessitates careful margin management. Understanding these discount trends helps in advising clients on competitive pricing, promotional planning, and potentially identifying categories where deeper discounts might be necessary to capture market share.

    14. Top 5 Products by Rating and Reviews
     - Method: Calculate Composite_Score = 0.6*rating + 0.4*log(rating_count), sort top 5.
     - Excel Pivot: Rows = product_name, category, Values = Composite_Score (Average), sort top 5.
     - Output:

![Task 14](https://github.com/user-attachments/assets/72bb5091-3a0f-4113-b405-4daef23d95a3)

Insights: The top products that excel in popularity (rating count) are: Electronics, Computers & Accessories and Home & Kitchen, While the products that have the highest customer satisfaction (Average Rating) are, Home improvements, Toys & Games and Office Products.
Elextronics stands out significantly with the highest combined score, reinforcing its position as a highly popular and well-regarded product.
Computer & Accessories also show strong performance, indicating a large, engaged, and satisfied customer base.
These products are invaluable assets for Amazon's clients. They represent flagship items that drive sales, build brand reputation, and foster customer loyalty due to their combination of high quality (High Average rating) and widespread adoption (high Rating count). Management should focus on maintaining the success of these products through continued quality assurance, active community engagement, and leveraging their popularity in marketing strategies (e.g., featuring them prominently, encouraging user-generated content).

---

### Recommendations
1. Optimize Pricing & Promotional Strategies:
   - Strategic Discounting: Advise clients to analyze the impact of deep discounts on profitability vs. sales volume,         especially in high-discount categories like Homeimprovements, Computer Accessories and Health & PersonalCare.            Encourage a nuanced approach where high-quality products might not need aggressive cuts.
   - Price Range Exploration: Investigate potential market demand and competitive landscape for products in the < ₹200        and ₹200-₹500 price ranges to identify untapped opportunities for product diversification.

2. Enhance Product Visibility & Customer Engagement:
   - Review Generation Campaigns: Implement targeted campaigns for the 309 products with fewer than 1,000 reviews to          boost their visibility and gather valuable customer feedback. This could include post-purchase email sequences,          incentivized reviews, or improved product descriptions.
   - Showcase Top Performers: Actively use the top 5 combined-score products (boAt, Redmi, etc.) in marketing campaigns       and storefronts as "bestsellers" or "customer favorites" to drive traffic and cross-selling.
     Continuous Monitoring & Adaptation:

3. Leverage Core Categories:
   - Invest Heavily in Electronics & Home & Kitchen: Given their market dominance in products, reviews, and potential         revenue, prioritize inventory, marketing, and new product development within these categories.
   - Analyze High-Rated Products: Study the attributes, marketing, and customer service strategies behind consistently        high-rated products (e.g., Electronics, Computers & Accessories) to replicate their success across other listings.

4. Continuous Monitoring & Adaptation:
   Regularly monitor key performance indicators (KPIs) related to sales, customer segments, shipping costs, and returns     to ensure ongoing strategic alignment and identify new opportunities or challenges.

---
### Data Visualization

