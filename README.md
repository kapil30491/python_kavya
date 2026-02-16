Amazon_Project
PROJECT 1: Data Cleaning Problem Statement
Problem Statement: Amazon Product Data Cleaning
The dataset contains Amazon product-level information including pricing, ratings, availability, delivery details, and promotional flags. Since the data is collected from web sources, it may contain:
•	Missing values
•	Incorrect data types
•	Duplicate records
•	Inconsistent price formats (currency symbols, commas, text)
•	Outliers in price, ratings, or sales volume
•	Boolean fields stored as text
•	Columns with irrelevant or redundant information
Objective
Clean and prepare the dataset to make it:
•	Consistent
•	Accurate
•	Analysis-ready
•	Suitable for visualization and business insights

Key Cleaning Tasks to Perform
Handle Missing Values
o	Check null values in each column
o	Impute or remove based on business logic
Fix Data Types
o	Convert price columns to numeric
o	Convert rating columns to float
o	Convert boolean flags (is_prime, is_best_seller, etc.) to True/False
o	Convert sales_volume to numeric
Clean Price Columns
o	Remove currency symbols ($, ₹, etc.)
o	Remove commas
o	Convert to float
Remove Duplicates
o	Based on asin (unique product identifier)
Outlier Detection
o	Detect extreme values in:
	product_price
	product_star_rating
	sales_volume
	product_num_ratings
Standardize Text Columns
o	Strip extra spaces
o	Convert categorical columns to consistent format
Feature Engineering (Optional but Strong Project Point)
o	Discount percentage
o	discount % = (original_price - product_price) / original_price * 100
o	Price difference
o	Rating category (High / Medium / Low)

PROJECT 2: Data Visualization Problem Statement
Problem Statement: Amazon Product Performance Analysis
After cleaning the dataset, perform exploratory data analysis (EDA) to identify patterns in pricing, ratings, discounts, and product performance.
The goal is to answer key business questions using visualizations.

Business Questions to Answer
Pricing Insights
•	What is the distribution of product prices?
•	Which price range has the most products?
•	Do Prime products have higher prices?
•	Are best sellers priced differently?
Ratings Analysis
•	What is the distribution of star ratings?
•	Do products with more ratings have better ratings?
•	Are Amazon’s Choice products highly rated?
Discount Analysis
•	Which products have highest discount?
•	Does higher discount increase sales volume?
•	Relationship between discount and rating?
Sales Performance
•	Do best sellers have higher sales volume?
•	Does Prime delivery affect sales?
•	Do products with more offers sell better?
Availability & Delivery
•	How many products are Prime eligible?
•	Are Prime products more likely to be best sellers?
•	Does fast delivery correlate with better ratings?
Competitive Analysis
•	Relationship between:
o	price vs rating
o	rating vs number of ratings
o	price vs sales volume

Recommended Visualizations in Jupyter
Univariate Analysis
•	Histogram → product_price
•	Histogram → product_star_rating
•	Countplot → is_prime
•	Countplot → is_best_seller
•	Boxplot → price (for outliers)
Bivariate Analysis
•	Scatterplot → price vs rating
•	Scatterplot → rating vs number of ratings
•	Boxplot → price by prime
•	Barplot → average rating by best seller
•	Barplot → sales volume by prime

Multivariate Analysis
•	Heatmap → correlation matrix
•	Pairplot (numeric columns)
•	Grouped barplot (prime + best seller)

Final Deliverables in Notebook
Your notebook should contain:
1.	Problem Statement
2.	Dataset Overview
3.	Data Cleaning Steps
4.	Outlier Handling
5.	Feature Engineering
6.	Exploratory Data Analysis
7.	Business Insights Summary
8.	Conclusion

