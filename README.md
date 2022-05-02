# Amazon_Vine_Analysis
Module 16

The pourpouse of this module is obtain:
1: Perform ETL on Amazon Product Reviews
2: Determine Bias of Vine Reviews

first we had to create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets (Links to an external site.), and extract the dataset into a DataFrame

The data that we select was:
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Toys_v1_00.tsv.gz

We upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

![image](https://user-images.githubusercontent.com/96089967/166342034-6c817313-41f3-404d-8b85-30860003e71c.png)




The processed database is read

![image](https://user-images.githubusercontent.com/96089967/166341104-00748956-c59a-402a-a2f5-d5218d1eb58e.png)





The data is filtered to create a DataFrame or table where there are 20 or more total votes
![image](https://user-images.githubusercontent.com/96089967/166341170-7388ee6d-c8af-42e5-894a-f46f53cf1c1f.png)





The data is filtered to create a DataFrame or table where the percentage of helpful_votes is equal to or greater than 50%
![image](https://user-images.githubusercontent.com/96089967/166341286-926bcd7b-2f6c-4146-96be-d3bf175d637b.png)





The data is filtered to create a DataFrame or table where there is a Vine review
![image](https://user-images.githubusercontent.com/96089967/166341329-9319cad3-2e55-480c-b093-1c48c123c4c4.png)




The data is filtered to create a DataFrame or table where there isn’t a Vine review
![image](https://user-images.githubusercontent.com/96089967/166341372-ca22b575-b2c6-44cd-b369-82ea9c913c4d.png)






The total number of reviews is 13320 Percentage: 94.07, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews is 15133 Percentage: 91.11
