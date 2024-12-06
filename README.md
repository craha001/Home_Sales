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
