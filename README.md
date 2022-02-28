Project Overview
•	The purpose of this project was to use "big data" to help Jennifer at Sellby to optimize their marketing efforts by comparing reviews they receive for the catalogue they offering compare to their competitors offering similar products.
•	 Sellby are also interested in enrolling in loyalty program that gives out free products to select reviewers based on the true review. They would like us to determine based on our analysis of "big data", if it is worth the cost. 
•	Since most of the reviews are in text format than numbers. It will be our job to convert them into numeric figures, analyze and present the findings.
•	This analysis was to be done using "Google Colab" to run the code, mainly using PySpark, a big data tool that was used for all data processing, Amazon Web Services (AWS) to store the data in the cloud, and pgAdmin to perform queries of the data locally.

Deliverable 1 – Perform ETL on Amazon Product Reviews
A snapshot of the code completed dataframes that were imported into their respective tables on pgAdmin 4 can be found below.
•	Customers Data-frame and Table
Customers Data-frame
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%201.3%20-%20customer_df.PNG
 
Customers Table
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%201.3.1-%20customer_table.PNG
 

•	Products Data-frame and Table
Products Data-frame
 https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%201.4-%20product_df.PNG
 
Products Table
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%201.4.1-%20product_table.PNG
 
•	Review ID Data-frame and Table
Review ID Data-frame
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%201.5-review_id_df.PNG
 
Review ID Table
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%201.5.1-%20review_id_table.PNG
 
•	Vine Data-frame and Table
Vine Data-frame
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%201.6-vine_df.PNG
 
Vine Table
 https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%201.6.1-vine_table.PNG
 









Deliverable 2 – Determining bias of Vine Reviews
•	Total Votes Count Equal To or Greater Than 20
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%202.4-%20Votes%20Greater%20than%2020.PNG
 


•	Percentage of Helpful Votes Greater Than 50%
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%202.1-%20Percentage%20of%20Helpful%20Votes%20Greater%20than%2050%25.PNG
 
•	Number Of Reviews Not Part of Vine (Unpaid) Program
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%202.2-%20Review%20Not%20Part%20of%20Vine%20Program.PNG

 










•	Analysis of Paid & Unpaid Reviews
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%202-%20Analysis%20of%20Paid%20%26%20Unpaid%20Reviews.PNG
 





Deliverable 3 - A Written Report on the Analysis
•	Purpose
•	The purpose of this challenge was to analyze Amazon reviews written by members of the paid Amazon Vine program. The dataset selected for analysis was the "Outdoors" dataset. 
•	The analysis involved using PySpark to perform the extract, transform, load (ETL) process to extract the data the dataset, transform the data and then connect to an AWS RDS instance, and load the transformed data into PGAdmin. 
•	Once the ETL process had been completed, PySPark was continued to be used for analysis to determine if there is any bias toward favorable reviews from Vine members in the "Outdoors" dataset.


•	Basis of Analysis
The analysis is done to find out the answers of the following questions
o	How many Vine reviews and non-Vine reviews were there?
o	What percentage of Vine reviews were 5 stars?. What percentage of non-Vine reviews were 5 stars?


•	Results
o	How many Vine reviews and non-Vine reviews were there?

1.	There was a total of 39,976 reviews consisting of both Vine and non-Vine reviews.
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%203.5-%20Total%20number%20of%20unpaid%20reviews.PNG
 
2.	There was a total of 107 Vine (paid) reviews.
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%203.3-Total%20Paid%20Reviews.PNG 

 
o	What percentage of Vine reviews were 5 stars?. What percentage of non-Vine reviews were 5 stars?
1.	The percentage 5 star reviews for Vine (paid) participants was 52.34%
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%203.1-%20Percentage%20of%205-Star%20Reviews%20for%20paid%20reviews.PNG
 

2.	The percentage of 5 star reviews of non-Vine (unpaid) participants was 52.69% 
https://github.com/sachinnabar/Amazon_Vine_Analysis/blob/main/Deliverable%203.2-%20Percentage%20of%205-star%20reviews%20for%20unpaid%20reviews.PNG
 
Summary
1.	Based on the results, we can conclude that there does not appear to be any positivity bias as to whether the paid Vine participants are producing more positive reviews of products compared to the non-Vine (unpaid) participants. A similar percentage of both paid and unpaid groups reviewed the products as 5 stars; in fact, a slightly greater portion of unpaid reviewers (52.69%), rated the products as 5 stars compared to only 52.34% of Vine members. Excluding statistical testing that could be done to determine if the sample sizes were large enough based on overall Vine participation, we can conclude that there does not appear to be any statistical positivity bias for Vine participants when it comes to providing 5 star reviews for the Outdoor products as there is a similar percentage of paid and unpaid reviewers who gave the products a 5 star review.
2.	To get accurate picture we have to consider another rating like 4 star or 3 star which is considered positive rating. Analyze 2 different data-frames and then come to a conclusion.

