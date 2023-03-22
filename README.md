# Amazon_Vine_Analysis
Module 17

## Analysis Overview
This project analyzes the Amazon Reviews written by members of the paid Vine program. This program is a service to manufacturers and publishers to receive reviews for their products. The companies will pay Amazon and provide products to Amazon Vine members, who then must review the products. I am interested in Video Gams, so I chose to review them. 
The analysis used Python's PySpark library to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into a postgreSQL database consisting of several tables, using pgAdmin4 on a Windows 10 platform and calculate different metrics as required. 

## Resources
* Data Source: Amazon Review datasets, Video Games Review dataset
* Software tools: Google Colab Notebooks, PostgreSQL 11.9, pgAdmin 4 version 6.19, AWS RDS Database Instance (access using jdbc)

## Results
Paid Vine Reviews Data:
* Total Vine reviews was 94 
* Total number of 5 star reviews, of these 94 reviews, 48 were 5-star
* Percentage 5 star reviews was about 51% or a little more than half being 5 star. 

We might want to know what products exactly were givne this high a rating, since I want to play those video games!

The image below shows the analysis code and results: <br>

<img src="https://github.com/valchau/Amazon_Vine_Analysis/blob/main/PaidVineReviewsData.PNG" alt="paid reviewer results" width="500" height="500" >
<br>

Non-Vine Reviews Data:
* Total Non-Vine reviews was 40,471, clearly a much larger number than the paid reviews.
* Total number of 5 star Non-Vine reviews, of this set of unpaid reviews, only 15,663 were 5 star.
* Percentage Non-Vine 5 star reviews was about 39%, which is more reasonable than the 51% above for the paid reviews.

<img src="https://github.com/valchau/Amazon_Vine_Analysis/blob/main/UnpaidReviewsData.PNG" alt=" non paid reviewer results" width="500" height="500" >
<br>


Summary
51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%.
The sample size of Vine reviews is very small compared to the non Vine reviews; however it does appear there might be a bias to give a 5 star review if you are a Vine member, since the 51% (proportion of 5 star reviews) is so much higher for this group than it is for the non Vine reviews. 
We might want to do a 2 proprotion t test to determine that these two samples come from different populations, as I suspect they do, but before doing that, I would recommend redoing the Vine review data with a much larger sample. 

