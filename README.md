Home Sales Analysis
This project involves analyzing home sales data using PySpark and SparkSQL. The analysis is done by answering specific queries related to home sales prices, taking advantage of PySpark's capabilities to handle large datasets efficiently.

Steps to Complete the Analysis

1. Rename the Notebook
Rename the Home_Sales_starter_code.ipynb file to Home_Sales.ipynb.
2. Import Required Libraries
Import the necessary PySpark SQL functions for the analysis.
3. Load the Data
Load the home_sales_revised.csv data into a Spark DataFrame.
4. Create a Temporary Table
Create a temporary table named home_sales from the DataFrame.
5. Perform Analysis with SparkSQL
   
Answer the following queries using SparkSQL:

Average Price for Four-Bedroom Houses by Year: Calculate and round to two decimal places.
Average Price for Homes with Three Bedrooms and Three Bathrooms by Year: Calculate and round to two decimal places.
Average Price for Homes with Specific Features by Year: (Three bedrooms, three bathrooms, two floors, and 2,000+ sq ft) Calculate and round to two decimal places.
Average Price per View Rating: For homes with an average price ≥ $350,000. Calculate the runtime and round to two decimal places.

7. Cache the Table
Cache the home_sales temporary table to improve query performance.

9. Verify the Cache
Check if the home_sales table is successfully cached.

11. Rerun Cached Query
Rerun the "Average Price per View Rating" query using cached data. Compare the runtime to the uncached version.

13. Partition the Data
Partition the data by date_built and save it in Parquet format.

15. Create Temporary Table from Parquet Data
Create a temporary table from the partitioned Parquet data.

17. Rerun Query on Parquet Data
Run the "Average Price per View Rating" query on the Parquet data. Compare the runtime to previous results.

19. Uncache the Table
Uncache the home_sales temporary table to free up resources.

21. Verify Uncache
Verify that the home_sales table is uncached.

23. Upload to GitHub
Download the Home_Sales.ipynb file and upload it to your "Home_Sales" GitHub repository.
