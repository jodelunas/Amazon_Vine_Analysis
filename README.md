# Amazon_Vine_Analysis

## Overview

For this project, I chose a data set of reviews on cameras.  I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. I used PySpark  to determine if there is any bias toward favorable reviews from Vine members. 


## Results

The vine table was filtered to create two new dataFrames for vine and unpaid reviews shown below.

### Vine Reviews

<img width="662" alt="VineReviews" src="https://user-images.githubusercontent.com/106006911/190466487-8d0a5207-2e9e-48c6-90ee-0619bfdbaeb9.png">

* Total Vine Reviews: 607
* Total 5 Star Reviews: 257
* Percent 5 Star Reviews: 42.34%
     
### Unpaid Reviews

<img width="679" alt="Unpaid_Reviews" src="https://user-images.githubusercontent.com/106006911/190466665-ab5c990c-5348-48fa-971e-f747c35db0f4.png">

* Total Unpaid Reviews: 50522
* Total 5 Star Reviews: 25220
* Percent 5 Star Reviews: 49.92%

## Summary

There doesn't seem to be a positivity bias for the reviews. The percentage of five star reviews is actually larger for unpaid reviews. To further confirm this, it would be important to also analize the one star reviews. Along with filtering for one star review, two through four would also be helpful. Having statistics on the whole range would make sure there isn't a bias between paid and unpaid.
