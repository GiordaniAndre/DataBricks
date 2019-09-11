# DataBricks
Resolved exercise from databricks course

Exercise 1: Perform an ETL Job

Write a basic ETL script that captures the 20 most active website users and load the results to DBFS.

Step 1: Create a DataFrame of Aggregate Statistics

Create a DataFrame ipCountDF that uses logDF to create a count of each time a given IP address appears in the logs, with the counts sorted in descending order. The result should have two columns: ip and count


Step 2: Save the Results

Use your tempory folder to save the results back to DBFS as ipCount.parquet


Exercise 2: Read Wikipedia Data 

Read Wikipedia data from Azure Blob Storage, accounting for its delimiter and header. 

 

Step 1: Get a Sense for the Data 

Take a look at the head of the data, located at /mnt/training/wikipedia/pageviews/pageviews_by_second.tsv. 

 

Step 2: Import the Raw Data 

Import the data without any options and save it to wikiDF. Display the result. 

 

Step 3: Import the Data with Options 

Import the data with options and save it to wikiWithOptionsDF. Display the result. Your import statement should account for: 
 
 

The header 

The delimiter 
