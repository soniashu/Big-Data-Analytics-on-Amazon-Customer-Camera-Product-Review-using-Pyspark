Big-Data-Analytics-on-Amazon-Customer-Reviews

Performed analysis using Pyspark, chaining, secondary sorting, partitioning, summarization, and filtration patterns. Also made use of Collaborative Filtering to build the recommendation system.

Abstract: Analysis of amazon is very crucial part when it comes to find an efficient way of getting insights on customer reviews about different products. Hence, this project is mainly aimed to analyse big data and produce an informative result about the customer reviews for the product Camera present on Amazon using Pyspark architecture, MLlib Collaborative Filtering and Optimized Storage.

Dataset:

Dataset Link: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Camera_v1_00.tsv.gz

Accessing the data: Data is present in the Amazon S3 bucket. It can be accessed as mentioned in below link, download the link and extract the Zip file – https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Camera_v1_00.tsv.gz About the data: DATA FORMAT - Tab ('\t') separated text file, without quote or escape characters. This dataset is 1GB in size. First line in the file is header; 1 line corresponds to 1 record.

DATA COLUMNS:

marketplace - 2 letter country code of the marketplace where the review was written.
customer_id - Random identifier that can be used to aggregate reviews written by a single author.
review_id - The unique ID of the review.
product_id - The unique Product ID the review pertains to. In the multilingual dataset the reviews for the same product in different countries can be grouped by the same product_id.
product_parent - Random identifier that can be used to aggregate reviews for the same product.
product_title - Title of the product.
product_category - Broad product category that can be used to group reviews (also used to group the dataset into coherent parts).
star_rating - The 1 to 5 star rating of the review.
helpful_votes - Number of helpful votes.
total_votes - Number of total votes the review received. vine - Review was written as part of the Vine program.
verified_purchase - The review is on a verified purchase.
review_headline - The title of the review.
review_body - The review text.
review_date - The date the review was written.
Data Analysis/Insights:

Find the total number of products present in the dataset.
Find the average product rating reviews for each product.
Find the topN reviewed products sorted by count.
Find total product rating for all those products which are present in the topN reviewed products.
Find all the users who has reviewed each product.
Find all the records partitioned by the date in which the product was reviewed.
Find all the product information for each unique star rating of the product by dividing it into different categories/bins.
Recommend the products to the user based on the star rating.
Find the count of the reviews grouped by date for each product.
Find the count of products for each product star rating.
Techniques/Technologies Used:

Pyspark and Databricks
Summarization Pattern – Numerical Summarization using Native Functions
Partitioning
Sorting
MLlib Recommendation System using Collaborative Filtering
