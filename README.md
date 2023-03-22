# Amazon_Vine_Analysis
Module 17

## Analysis Overview
This project analyzes the Amazon Reviews written by members of the paid Vine program. This program is a service to manufacturers and publishers to receive reviews for their products. The companies will pay Amazon and provide products to Amazon Vine members, who then must review the products. I am interested in Video Gams, so I chose to review them. 
The analysis used Python's PySpark library to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into a postgreSQL database consisting of several tables, using pgAdmin4 on a Windows 10 platform and calculate different metrics as required. 

## Resources
•	Data Source: Amazon Review datasets, Video Games Review dataset
•	Software: Google Colab Notebooks, PostgreSQL 11.9, pgAdmin 4 version 6.19, AWS RDS Database Instance

##Results
Total number of reviews
•	Vine reviews
 


•	Non-Vine reviews
 


Total number of 5-star reviews
•	Vine reviews
 


•	Non-Vine reviews
 


Percentage of 5-star reviews
•	Vine reviews
 


•	Non-Vine reviews
 


Summary
51% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is only 39%.
This describes a likely bias for more positive reviews in the Vine program.
If more information and details are needed, we could analyse the statistical information (mean, median and mode) of the star rating for the Vine and non-Vine reviews.

