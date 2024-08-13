Home Sales Analysis

This project focuses on analyzing home sales data using PySpark and SparkSQL. The goal is to gain insights into various trends and patterns in home prices by leveraging the efficiency of PySpark in handling large datasets. The analysis addresses specific queries related to home sales prices, helping to uncover valuable information about the real estate market.

Project Overview

In this project, you will work through a series of tasks that involve data preparation, analysis, and optimization. You’ll explore how caching and partitioning can improve the performance of SparkSQL queries, especially when working with large datasets. The project is structured to guide you through each step, ensuring a thorough understanding of the process.

Instructions

1. File Renaming
Task: Rename the Home_Sales_starter_code.ipynb file to Home_Sales.ipynb.
2. Import Libraries
Task: Import the necessary PySpark SQL functions required for this assignment. These functions will be used to perform SQL queries and manage data efficiently.
3. Load Data
Task: Load the home_sales_revised.csv data file into a Spark DataFrame. This DataFrame will serve as the basis for your analysis.
4. Create Temporary Table
Task: Create a temporary table named home_sales from the DataFrame. This table will allow you to execute SQL queries on the dataset.
5. Analysis Using SparkSQL
Task: Answer the following questions using SparkSQL:

Average Price for Four-Bedroom Houses by Year

Query: Calculate the average price for a four-bedroom house sold each year. Round your answer to two decimal places.
Average Price for Homes with Specific Features by Year

Query: Calculate the average price of homes built in each year that have three bedrooms and three bathrooms. Round your answer to two decimal places.
Average Price for Homes with Additional Features by Year

Query: Calculate the average price of homes built in each year that have three bedrooms, three bathrooms, two floors, and a living area of 2,000 square feet or more. Round your answer to two decimal places.
Average Price per View Rating

Query: Calculate the average price of homes per "view" rating, where the average home price is greater than or equal to $350,000. Measure the runtime for this query, and round your answer to two decimal places.
6. Caching the Table
Task: Cache the home_sales temporary table to improve query performance. Caching allows Spark to store the data in memory, reducing the time needed to retrieve it for subsequent queries.

7. Verify Cache Status
Task: Check whether the home_sales temporary table is successfully cached. This step ensures that the data is stored in memory for faster access.

9. Run Cached Query
Task: Using the cached data, rerun the query that calculates the average price of homes per "view" rating with an average home price greater than or equal to $350,000. Measure the runtime and compare it to the uncached runtime to evaluate the performance improvement.

11. Partitioning Data
Task: Partition the data by the date_built field and save it in Parquet format. Partitioning helps to organize the data in a way that improves query performance, especially when filtering on the partitioned field.

13. Create Temporary Table for Parquet Data
Task: Create a temporary table from the partitioned Parquet data. This allows you to perform SQL queries on the optimized dataset.

15. Run Query on Parquet Data
Task: Run the query that calculates the average price of homes per "view" rating, with an average home price greater than or equal to $350,000, on the Parquet data. Measure the runtime and compare it to the previous runtimes to observe the effects of partitioning.

17. Uncache the Temporary Table
Task: Uncache the home_sales temporary table to free up memory resources once you’ve completed your analysis.

19. Verify Uncache Status
Task: Verify that the home_sales temporary table is uncached using PySpark. This step confirms that the data is no longer stored in memory.

21. Upload to GitHub
Task: Download the Home_Sales.ipynb file and upload it to your "Home_Sales" GitHub repository. This ensures that your work is saved and accessible for future reference.
