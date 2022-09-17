# Amazon_Vine_Analysis

## Overview of Amazon_Vine_Analysis
For this project, we used Google Colab, PySpark, AWS (S3 and RDS), PostgreSQL, and pgAdmin to analyse Amazon reviews from members of the paid Amazon Vine program. Picking one of many possible datasets (the furniture data), I used PySpark to perform the ETL process, and then connected to an AWS RDS instance, and dumped the data into pgAdmin. Finally, I re-extracted the data from pgAdmin with PySPark and analysed the dataset to determine if there was any bias towards Vine members.

## Results
By filtering the Furniture dataset, I was able to produce the following results:

![Results](https://user-images.githubusercontent.com/106599446/190832395-5568b9d5-4eb6-4936-a4ac-43ba58ba3521.png)

As visible in the image above, there were 130 Vine reviews, and 789,338 non-vine reviews. Of these groups, there were 70 5-star vine reviews, and 446,360 non-vine 5-star reviews. That equates to 53.85% and 56.55% of the totals, respectively. 

## Summary
As seen in the data above, there is no clear bias for vine reviews as compared to the non-vine reviews. In fact, there was a higher percentage of non-vine 5-star reviews than there were 5-star vine reviews. To analyse the possibility of bias further, I recommend reviewing the percentage difference in lower review tiers; it is possible that vine reviewers are not as inclined to leave a negative rating as compared to non-vine reviewers.
