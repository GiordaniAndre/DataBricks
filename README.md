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



Exercise 03: Exploring JSON Data
Smartphone data from UCI Machine Learning Repository is available under /mnt/training/UbiqLog4UCI. This is log data from the open source project Ubiqlog.

Import this data and define your own schema.

Step 1: Import the Data
Import data from /mnt/training/14_F/log*. (This is the log files from a given user.)

Look at the head of one file from the data set. Use /mnt/training/UbiqLog4UCI/14_F/log_1-6-2014.txt.

Step 2: Explore the Inferred Schema

Print the schema to get a sense for the data.

Exercise 04: Creating a User Defined Schema

Step 1: Set Up Your workflow. Often the hardest part of a coding challenge is setting up a workflow to get continuous feedback on what you develop.

Start with the import statements you need, including functions from two main packages:

Step 2: Create the Full Schema for SMS
Define the Schema for the following fields in the StructType SMS and name it schema2. Apply it to a new DataFrame SMSDF2:


Address

date

metadata


Step 3: Compare Solution Performance

Compare the dafault schema inference to applying a user defined schema using the %timeit function. Which completed faster? Which triggered more jobs? Why?

Exercise 05:Working with Corrupt Records

Step 1: Diagnose the Problem

Import the data used in the last lesson, which is located at /mnt/training/UbiqLog4UCI/14_F/log*. Import the corrupt records in a new column SMSCorrupt.

Save only the columns SMS and SMSCorrupt to the new DataFrame SMSCorruptDF.

Step 2: Use badRecordsPath

Use the badRecordsPath option to save corrupt records to the directory /tmp/corruptSMS.
