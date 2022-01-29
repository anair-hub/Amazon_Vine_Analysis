# Amazon_Vine_Analysis

## Overview
  There are approximately 50 datasets and each one contains reviews of a specific product, from clothing apparel to wireless products. We will use on of the dataset and 
use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset. 


## Results
Deliverable 1
1-Pick a dataset from Amazon review dataset and extract the same into a dataframe
2-Transfor the dataframe into four separate Dataframes that match the table schema in pgAdmin
3-Upload transformed data into the appropriate tables and run queries in pgAdmin to confirm that data has been uploaded
 
![Del1_Table_Creation](Images/Del1_Table_Creation-pgadmin.PNG)

![Customer_dataframe](Images/Customer_dataframe.PNG)

![Products_Dataframe](Images/Products_Dataframe.PNG)

![Review_Dataframe](Images/Review_Dataframe.PNG)

![Vine_Dataframe](Images/Vine_Dataframe.PNG)

![Customer-table](Images/Customer-table.PNG)

![Products-table](Images/Products-table.PNG)

![Review_Id_Table](Images/Review_Id_Table.PNG)

![Vine-table](Images/Vine-table.PNG)

Deliverable 2

1-Method Used- Using PySpark
2-The data is filtered to create a DataFrame or table where there are 20 or more total votes 
3-The data is filtered to create a DataFrame or table where the percentage of helpful_votes is equal to or greater than 50% 
4-The data is filtered to create a DataFrame or table where there is a Vine review  
5-The data is filtered to create a DataFrame or table where there isn’t a Vine review  
6-The total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews  

 

![Vine_20](Images/Vine_20.PNG) 

![Vine_50](Images/Vine_50.PNG) 

![Vine_Paid](Images/Vine_Paid.PNG) 

![Vine_Unpaid](Images/Vine_Unpaid.PNG) 
 
![Reviews_Paid_Percentage](Images/Reviews_Paid_Percentage.PNG) 

![Reviews_Unpaid_Percentage](Images/Reviews_Unpaid_Percentage.PNG) 

Questions:

How many Vine reviews and non-Vine reviews were there?
question1a.PNG
question1b.PNG

![question1a](Images/question1a.PNG) 

![question1b](Images/question1b.PNG) 

There were total of 94 paid reviews and 40,471 count of unpaid reviews

How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![question2a](Images/question2a.PNG) 

![question2b](Images/question2b.PNG) 

There were total of 48 paid reviews with 5 stars and 15,663 count of unpaid reviews with 5 stars

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![question3a](Images/question3a.PNG) 

![question3b](Images/question3b.PNG) 

51% of paid vine reviews were 5 stars and for unpaid vine reviews it was 39%

## Summary

![question4a](Images/question4a.PNG) 

![question4b](Images/question4b.PNG) 

Total reviews were 40,565 and of that 15,711 were 5 starts which makes it upto 39 percent. Based on the results, there seems to be no positivity bias for the Vine program at all. 
On furthur classification it can be seen that 51% of paid vine reviews were 5 stars and for unpaid vine reviews it was 39%. This shows that there was positive bias in the vine program.

Additional data attribute that could have helped in analysis is inclusion of the verified purchase data.




