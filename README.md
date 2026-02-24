# 📖**Amazon Sales Dataset Analysis**

## **Project Overview :**

This Google Colab notebook provides a comprehensive analysis of Amazon product sales data, focusing on product information, customer reviews, and sentiment analysis. The analysis includes data cleaning, exploratory data analysis (EDA), statistical testing, and sentiment analysis of customer reviews.

## **Dataset :**
The dataset is sourced from Kaggle: https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset and This dataset is having the data of 1K+ Amazon Product's Ratings and Reviews as per their details listed on the official website of Amazon

## **Features:**

- product_id - Product ID
- product_name - Name of the Product
- category - Category of the Product
- discounted_price - Discounted Price of the Product
- actual_price - Actual Price of the Product
- discount_percentage - Percentage of Discount for the Product
- rating - Rating of the Product
- rating_count - Number of people who voted for the Amazon rating
- about_product - Description about the Product
- user_id - ID of the user who wrote review for the Product
- user_name - Name of the user who wrote review for the Product
- review_id - ID of the user review
- review_title - Short review
- review_content - Long review
- img_link - Image Link of the Product
- product_link - Official Website Link of the Product

## **Features Analyzed :**

 ### 🔓**Data Processing:**

* Splitting data into two main DataFrames:
  
  - products_df: Contains product-level information (1,465 rows × 11 columns)
  - reviews_df: Contains review-level information (1,465 rows × 6 columns)
    
* Data type conversions for numeric fields (prices, ratings, discount percentages)
* Handling missing values using category-based median imputation
* Category column parsing into hierarchical levels (main_category, sub_category_1 through sub_category_4)


 ### 📊**Exploratory Data Analysis (EDA) :**
 
The notebook includes comprehensive EDA with visualizations:
**Price Analysis:**
  * Distribution of actual and discounted prices
  * Identification of most and least expensive products
  * Relationship between actual and discounted prices
  * Discount percentage distribution across products

**Rating Analysis:**
  * Product rating distribution
  * Top 10 most-rated products
  * Correlation between price and rating

**Category Analysis:**
  * Average price per main category
  * Average discount percentage per category


### 💵**Statistical Tests :**

* T-test: Comparing ratings between product categories (electronics vs. clothing)
* Chi-square test: Analyzing relationship between actual price and rating categories

### 🧐**Sentiment Analysis :**
 
Using TextBlob library to analyze customer reviews:
* Text cleaning (lowercase conversion, URL removal, special character removal).
* Polarity and subjectivity scoring for each review.
* Sentiment classification (Positive, Neutral, Negative).
* Product-level sentiment aggregation (average polarity, positive review ratio).
* Sentiment distribution analysis (93% positive, 6.6% neutral, 0.4% negative).

## **Key Findings**
* Product Distribution: Wide range of product prices from ₹39 to ₹139,900
* Rating Patterns: Most products are well-rated (average rating ~4.1)
* Discount Trends: Home Improvement and Computers & Accessories categories offer highest average discounts
* Customer Sentiment: Overwhelmingly positive customer feedback (93% positive reviews)
* Category Performance: Electronics dominates the dataset with most products and highest-priced items

## **Author**
This analysis was developed as part of a mini data science project to demonstrate data cleaning, EDA, statistical analysis, and sentiment analysis techniques using real-world e-commerce data.

