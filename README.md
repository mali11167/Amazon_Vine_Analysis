# Amazon_Vine_Analysis
## Overview
This project is to analyze Amazon reviews written by members of the paid Amazon Vine program. There are a lot of dataseta available to review.
I chose to review the Major Appliances dataset. This dataset gives us the overview of the product id, description of a particular product, number
of reviews on each item, and the star ratings. 
## Results
I used Google Colab and PySpark for this project. This dataset was a pretty big dataset so we performed a few filters to get what we needed. 
First we did  a count on customer id to see how many customer are in the dataset and below are the results:

![customer](https://user-images.githubusercontent.com/91965321/153692793-358fc897-8b69-49a7-9a44-a6a0fa6f707b.PNG)

We filtered the product information through product id and product title and below is the result for it

![product](https://user-images.githubusercontent.com/91965321/153692810-908ae784-0fd2-4b4f-8a5b-97ba1bb24877.PNG)

We then filtered to get review table based on review id, customer id, product id, product parent and review date as below is the result

![review](https://user-images.githubusercontent.com/91965321/153692815-0cd084b4-a7f1-44a5-8d4b-86186ddbf97d.PNG)

Finally we created a vine table based on review id, star rating and voting as follows

![vine](https://user-images.githubusercontent.com/91965321/153692827-a19c0f40-ba6e-4249-a1ee-611ba1148498.PNG)

Looking at the vine program following are my findings on it;
* Number of vine reviews were 35
* Number of non vine reviews were 4957
* Number 5 star rating in vine reviews is 18
* Number of 5 star rating in non vine review is 1963
* The percentage of Vine reviews for 5 stars is 51%
* The percentage of Non Vine reviews for 5 star is 39%

Below is the detail of the results:
![count](https://user-images.githubusercontent.com/91965321/153691618-0d91f6c7-4ccd-4afc-a50a-301bc44374c7.PNG)
![percentage](https://user-images.githubusercontent.com/91965321/153691621-3dd74bfa-d8ce-446d-8953-ee83d7fe7761.PNG)

## Summary
According to the analysis that was done I think the vine program results are not bias as number of paid reviews were very less as
compared to non paid reviews. The non paid reviews are actually the one that gave their honest opinion based on there experience with
the product or the performance of the product. 
Another analysis we can do to support the analysis take in count for the reviews for only the customers that have a verified purchase. There
should be an option at the time of purchase to register the product. This was ther purchase will be verified and the review in regards to that
purchase will be verified. This would eliminate any non related and fake reviews. 






