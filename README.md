# DataBricks
Resolved exercise from databricks course

Exercise 1: Perform an ETL Job

Write a basic ETL script that captures the 20 most active website users and load the results to DBFS.

Step 1: Create a DataFrame of Aggregate Statistics

Create a DataFrame ipCountDF that uses logDF to create a count of each time a given IP address appears in the logs, with the counts sorted in descending order. The result should have two columns: ip and count


Step 2: Save the Results

Use your tempory folder to save the results back to DBFS as ipCount.parquet
