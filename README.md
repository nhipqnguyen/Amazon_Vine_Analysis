# Amazon_Vine_Analysis
## Overview of the analysis
- This project analyzes Amazon reviews of products in the category "Shoes" written by members of the paid Amazon Vine program. We use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, we use PySpark to determine if there is any bias toward favorable reviews from Vine members the dataset.
- Data resource: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Shoes_v1_00.tsv.gz
## Results
- Below is the summary table for the Vine reviews:

  ![paid summary](https://github.com/nhipqnguyen/Amazon_Vine_Analysis/blob/main/analysis/paid_summary.png)

- Below is the summary table for the non-Vine reviews:

  ![unpaid summary](https://github.com/nhipqnguyen/Amazon_Vine_Analysis/blob/main/analysis/unpaid_summary.png)

## Summary
- As shown in the above tables, the percentages of 5-star reviews for the paid and unpaid types are 59.1% and 53.6%, respectively. The 5-star reviews account for a slightly higher percentage of all paid reviews than they do in the unpaid group. However, this difference is not significant considering the difference in size of 2 groups. Therefore, there is no significant bias for reviews for shoes products in the Vine program. 
- Below is the comparison of the average rating of the products that were rated in both Vine and non-Vine groups:
  
  ![avg_rating_paid_vs_unpaidy](https://github.com/nhipqnguyen/Amazon_Vine_Analysis/blob/main/analysis/avg_rating_paid_vs_unpaid.png)

 - Out of the 5 products that were rated in both groups, only 1 shows significant difference between the ratings (4.5 vs. 1). That being said, there is no significant bias for shoes products' review between the Vine and non-Vine groups.