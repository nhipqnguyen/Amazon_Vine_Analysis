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
state if there is any positivity bias for reviews in the Vine program.Then, provide one additional analysis that you could do with the dataset to support your statement
- The summary states whether or not there is bias, and the results support this statement (2 pt)
- An additional analysis is recommended to support the statement