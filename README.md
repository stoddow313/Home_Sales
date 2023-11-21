# Home_Sales

## Background: 

In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Instructions: 

1. Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.

2. Import the necessary PySpark SQL functions for this assignment.

3. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.

4. Create a temporary table called home_sales.

5. Answer the following questions using SparkSQL:

    - What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

    - What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

    - What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

    - What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

6. Cache your temporary table home_sales.

7. Check if your temporary table is cached.

8. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

9. Partition by the "date_built" field on the formatted parquet home sales data.

10. Create a temporary table for the parquet data.

11. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

12. Uncache the home_sales temporary table.

13. Verify that the home_sales temporary table is uncached using PySpark.

14. Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.

## Answers to above questions: 

1. The average price for a 4 bedroom home sold each year: 
    - 2022: $296,363.88
    - 2021: $301,819.44
    - 2020: $298,353.78
    - 2019: $300,263.70
2. The average price of a 3 bed, 3 bath home: 
    - 2017: $292,676.79
    - 2016: $290,555.07
    - 2015: $288,770.30
    - 2014: $290,852.27
    - 2013: $295,962.27
    - 2012: $293,683.19
    - 2011: $291,117.47
    - 2010: $292,859.62
3. Average price of a 3 bed, 3 bath, 2 floor home: 
    - 2017: $280,317.58
    - 2016: $293,965.10
    - 2015: $297,609.97
    - 2014: $298,264.72
    - 2013: $303,676.79
    - 2012: $307,539.97
    - 2011: $276,553.81
    - 2010: $285,010.22
4. View rating from homes costing greater than or equal to $350,000: 
    - 51: $788,128.21
    - 54: $798,684.82
    - 69: $750,537.94
    - 87: $1,072,285.20
    - 73: $752,861.18
    - 64: $767,036.67
    - 59: $791,453.00
    - 85: $1,056,336.74
    - 52: $733,780.26
    - 71: $775,651.10
    - 98: $1,053,739.33
    - 99: $1,061,201.42
    - 96: $1,017,815.92
    - 100: $1,026,669.50
    - 70: $695,865.58
    - 61: $746,877.59
    - 75: $1,114,042.94
    - 78: $1,080,649.37
    - 89: $1,107,839.15
    - 77: $1,076,205.56