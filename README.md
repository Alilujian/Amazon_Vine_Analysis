# Amazon_Vine_Analysis

## Overview
This project analyze Amazon reviews written by members of paid Amazon Vine program. By accessing the video game review dataset, we use PySpark to perform the ETL process to extract the datset, transform the data, and connect to an AWS RDS instance, and finaly load the transformed data into pgAdmin for further analysis.
At the end we will use PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset.

### Data Source:
* Video Games Review Datasets[https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz]

## Results
### Total Number of Reviews
* Total reviews\
![total_reviews](Resources/total_reviews.png)

*  Vine member reviews\
![paid_reviews](Resources/paid_reviews.png)

* Non-Vine member reviews\
![unpaid_reviews](Resources/unpaid_reviews.png)

### 5-Star Reviews
* Total 5-Star Reviews\
![total_5star](Resources/total_5star.png)
* Vine member reviews\
![5_star_paid](Resources/5_star_paid.png)
* Non-Vine member reviews\
![unpaid_5star](Resources/unpaid_5star.png)

### 5-Star Review Percentage
* Total percentage\
![5star_percent](Resources/5star_percent.png)

*  Vine member reviews\
![paid_percent](Resources/paid_percent.png)

* Non-Vine member reviews\
![unpaid_percent](Resources/unpaid_percent.png)

## Summary
The 5-star reviews percentage for Vine progream were 51% while the percentage in non-program user were only about 38%. This indicates a bias for reviews by user of the Vine program. If we look at the 5-star percentage in the entire dataset, the number was 38% which is similar to the non-Vine program percentage. This indicates that the bias for Vine program might not have significant impact on the entire dataset.
