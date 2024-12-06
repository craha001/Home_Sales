# Module 22 Challenge Home_Sales
For this week's challenge, I use SparkSQL to determine key metrics for home sales data. In doing so, I created temporary views, partitioned the data, cache and uncache a temporary table, and finally verify the table has been uncached.  
The code for my work is found in the Home_Sales file in this repository.

## Dependencies Imported
import findspark  
findspark.init()  
from pyspark.sql import SparkSession  
import time  
from pyspyark import SparkFiles  

## Analysis Questions 
1. What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.  
![image](https://github.com/user-attachments/assets/6f6cb1a9-3570-4c6e-abe3-ed277770e1f3)  

2. What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.  
![image](https://github.com/user-attachments/assets/73e0d106-7411-4cdf-a3a6-4e830b41ed29)  

3. What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.  
![image](https://github.com/user-attachments/assets/05d29c11-7167-48e1-8294-f2512dc1c705)

4. What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
   ![image](https://github.com/user-attachments/assets/931d6e0f-aa81-4cce-9094-b64a4acbe557)

## SparkSQL run times for Uncached table, Cached table, and Parquet table of analysis question 4 SQL Query
Uncached  = 1.114 seconds  
Cached = 0.574 seconds  
Parquet = 0.501 seconds  
Clearly the Parquet table had the fastest run time however it is fairly close to the Cached table run time.


