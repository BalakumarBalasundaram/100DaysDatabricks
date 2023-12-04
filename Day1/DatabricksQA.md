 
# Questions 
 
# 1. Databricks Architecture & Services
   
1.1. What are the two main components of the Databricks Architecture?
   
1.2. What are the three different Databricks services? 

1.3. What is a cluster? 

1.4. What are the two cluster types? 

1.5. How long does Databricks retain cluster configuration information? 

1.6. What are the three cluster modes?  

1.7. Cluster size and autoscaling  

1.8. What is local disk encryption? 

1.9. What are the cluster security modes?

1.10. What is a Pool? 

1.11. What happens when you terminate / restart / delete a cluster? 

# 2. Basic Operations for Databricks Notebooks

2.1. Which magic command do you use to run a notebook from another notebook? 

2.2. What is Databricks utilities and how can you use it to list out directories of files from Python cells? 

2.3. What function should you use when you have tabular data returned by a Python cell? 

# 3. Git Versioning with Databricks Repos

3.1. What is Databricks Repos? 

3.2. What are the recommended CI/CD best practices to follow when developing with Repos?  

# 4. Delta Lake and the Lakehouse
   
4.1. What is the definition of a Delta Lake?
   
4.2. How does Delta Lake address the data lake pain points to ensure reliable, ready-to-go data?

4.3. Describe how Delta Lake brings ACID transactions to object storage 

4.4. Is Delta Lake the default for all tables created in Databricks?

4.5. What data objects are in the Databricks Lakehouse?

4.6. What is a metastore?

4.7. What is a catalog?

4.8. What is a Delta Lake table?

4.9. How do relational objects work in Delta Live Tables?

# 5. Managing Delta Tables
   
5.1. What is the syntax to create a Delta Table?
   
5.2. What is the syntax to insert data?

5.3. Are concurrent reads on Delta Lake tables possible?

5.4. What is the syntax to update particular records of a table?

5.5. What is the syntax to delete particular records of a table?

5.6. What is the syntax for merge and what are the benefits of using merge? 

5.7. What is the syntax to delete a table? 

# 6. Advanced Delta Lake Features

6.1. What is Hive? 

6.2. What are the two commands to see metadata about a table? 

6.3. What is the syntax to display the Delta Lake files? 

6.4. Describe the Delta Lake files, their format and directory structure  

6.5. What does the query engine do using the transaction logs when we query a Delta Lake table?  

6.6. What commands do you use to compact small files and index tables?  

6.7. How do you review a history of table transactions? 

6.8. How do you query and roll back to previous table version?    

6.9. What command do you use to clean up stale data files and what are the consequences of using this 
command? 

6.10. Using Delta Cache  

# 7. Databases and Tables on Databricks
   
7.1. What is the syntax to create a database with default location (no location specified)? 

7.2. What is the syntax to create a database with specified location?  

7.3. How do you get metadata information of a database? Where are the databases located (difference between default vs custom location)  

7.4. What's the best practice when creating databases?  

7.5. What is the syntax for creating a table in a database with default location and inserting data? What is the syntax for a table in a database with custom location?  

7.6. Where are managed tables located in a database and how can you find their location?

7.7. What is the syntax to create an external table?

7.8. What happens when you drop tables (difference between a managed and an unmanaged table)?

7.9. What is the command to drop the database and its underlying tables and views?

# 8. Views and CTEs on Databricks

8.1. How can you show a list of tables and views?

8.2. What is the difference between Views, Temp Views & Global Temp Views?

8.3. What is the syntax for each? 

8.4. Do views create underlying files?

8.5. Where are global temp views created? 

8.6. What is the syntax to select from global temp views?  

8.7. What are CTEs? What is the syntax? 

8.8. What is the syntax to make multiple column aliases using a CTE?  

8.9. What is the syntax for defining a CTE in a CTE?  

8.10. What is the syntax for defining a CTE in a subquery?  

8.11. What is the syntax for defining a CTE in a subquery expression  

8.12. What is the syntax for defining a CTE in a CREATE VIEW statement?   

# 9. Extracting Data Directly from Files

9.1. How do you query data from a single file?  

9.2. How do you query a directory of files?  

9.3. How do you create references to files?  

9.4. How do you extract text files as raw strings?  

9.5. How do you extract the raw bytes and metadata of a file? What is a typical use case for this?  

# 10. Providing Options for External Sources

10.1. Explain why executing a direct query against CSV files rarely returns the desired result.  

10.2. Describe the syntax required to extract data from most formats against external sources.  

10.3. What happens to the data, metadata and options during table declaration for these external sources?  

10.4. Does the column order matter if additional csv data files are added to the source directory at a later stage? 

10.5. What is the syntax to show all of the metadata associated with the table definition?  

10.6. What are the limits of tables with external data sources?  

10.7. How can you manually refresh the cache of your data?  

10.8. What is the syntax to extract data from SQL Databases?  

10.9. Explain the two basic approaches that Spark uses to interact with external SQL databases and their limits  

# 11. Creating Delta Tables
  
11.1. What is a CTAS statement and what is the syntax?

11.2. Do CTAS support manual schema declaration?  

11.3. What is the syntax to overcome the limitation when trying to ingest data from CSV files?  

11.4. How do you filter and rename columns from existing tables during table creation?  

11.5. What is a generated column and how do you declare schemas with generated columns?  

11.6. What are the two types of table constraints and how do you display them?  

11.7. Which built-in Spark SQL commands are useful for file ingestion (for the select clause)?  

11.8. What are the three options when creating tables?  

11.9. As a best practice, should you default to partitioned tables for most use cases when working with Delta Lake?  

11.10. What are the two options to copy Delta Lake tables and what are the use cases?  

# 12. Writing to Delta Tables

12.1. What are the multiple benefits of overwriting tables instead of deleting and recreating tables?  

12.2. What are the two easy methods to accomplish complete overwrites?  

12.3. What are the differences between the two?  

12.4. What is the syntax to atomically append new rows to an existing Delta table? Is the command idempotent?  

12.5. What is the syntax for the the MERGE SQL operation and the benefits of using merge?   

12.6. How can you use merge for deduplication?  

12.7. What is the syntax to have an idempotent option to incrementally ingest data from external systems?  

12.8. How is COPY INTO different than Auto Loader?   

# 13. Cleaning Data

13.1. Do COUNT and DISTINCT queries skip or count nulls?  

13.2. What is the syntax to count null values?  

13.3. What is the syntax to count for distinct values in a table for a specific column? 

13.4. What is the syntax to cast a column to valid timestamp?  

13.5. What is the syntax for regex?  

# 14. Advanced SQL Transformations

14.1. What is the syntax to deal with binary-encoded JSON values in a human readable format? 

14.2. What is the Spark SQL functionality to directly interact with JSON data stored as strings?

14.3. What are struct types? What is the syntax to parse JSON objects into struct types with Spark SQL?  

14.4. Once a JSON string is unpacked to a struct type, what is the syntax to flatten the fields into columns?  What is the syntax to interact with the subfields in a struct type?  

14.5. What is the syntax to deal with nested struct types?  

14.6. What is the syntax for exploding arrays of structs?  

14.7. What is the syntax to collect arrays?  

14.8. What is the syntax for an INNER JOIN ?   

14.9. What is the syntax for an outer join?  

14.10. What is the syntax for a left/right join?  

14.11. What is the syntax for an anti-join?  

14.12. What is the syntax for a cross-join?  

14.13. What is the syntax for a semi-join? 

14.14. What is the syntax for the Spark SQL UNION , MINUS , and INTERSECT set operators?   

14.15. What is the syntax for pivot tables?  

14.16. What are higher order functions? ( FILTER , EXIST , TRANSFORM , REDUCE )?   

14.17. What is the syntax for FILTER ?  

14.18. What is the syntax for EXIST ?   

14.19. What is the syntax for TRANSFORM ?   

14.20. What is the syntax for REDUCE ?   

# 15. SQL UDFs and Control Flow

15.1. What is the syntax to define and register SQL UDFs? How do you then apply that function to the data?  

15.2. How can you see where the function was registered and basic information about expected inputs and what is returned?  

15.3. What are SQL UDFs governed by?  

15.4. What permissions must a user have on the function to use a SQL UDF? Describe their scoping.  

15.5. What is the syntax used for the evaluation of multiple conditional statements?  

15.6. What is the syntax using SQL UDFs for custom control flow within SQL workloads?  

15.7. What is the benefit of using SQL UDFs?  


# 16. Python for Databricks SQL & Python Control Flow

16.1. What is the syntax to turn SQL queries into Python strings?  

16.2. What is the syntax to execute SQL from a Python cell?  

16.3. What function do you call to render a query the way it would appear in a normal SQL notebook?  

16.4. What is the syntax to define a function in Python?  

16.5. What is the syntax for f-strings?  

16.6. How can f-strings be used for SQL queries?  

16.7. What is the syntax for if / else clauses wrapped in a function?   

16.8. What are the two methods for casting values to numeric types (int and float)?  

16.9. What are assert statements and what is the syntax?   

16.10. Why do we use try / except statements and what is the syntax?   

16.11. What is the downside of using  try / except statements?   

16.12. What is the syntax for try / except statements where you return an informative error message?   

16.13. How do you apply these concepts to execute SQL logic on Databricks, for example to avoid SQL injection attack?  

# 17. Incremental Data Ingestion with Auto Loader

17.1. What is incremental ETL? 

17.2. What is the purpose of Auto Loader?

17.3. What are the 4 arguments using Auto Loader with automatic schema inference and evolution?  

17.4. How do you begin an Auto Loader stream?

17.5. What is the benefit of Auto Loader compared to structured streaming?

17.6. What keyword indicates that you're using Auto Loader rather than a traditional stream for ingesting?  

17.7. What can you do once data has been ingested to Delta Lake with Auto Loader?  

17.8. What is the _rescued_data column?  

17.9. What is the data type encoded by Auto Loader for fields in a text-based file format?  

17.10. Historically, what were the two inefficient ways to land new data?  

17.11. Is there a delay when records are ingested with an Auto Loader query?  

17.12. How do you track the ingestion progress?  

# 18. Reasoning about Incremental Data with Spark Structured Streaming

18.1. What is Spark Structured Streaming?  

18.2. What were the traditional approaches to data streams?  

18.3. Describe the programming model for Structured Streaming.  

18.4. Explain how Structured Streaming ensures end-to-end exactly-once fault-tolerance. 

18.5. What is the syntax to read a stream?  

18.6. How can you transform streaming data?  

18.7. Give an example operation that is not possible when working with streaming data. What methods can you use to circumvent these exceptions?  

18.8. How do you persist streaming results?  

18.9. What are the 3 most important settings when writing a stream to Delta Lake tables?  

18.10. What is the syntax to load data from a streaming temp view back to a DataFrame, and then query the table that we wrote out to?  

# 19. Incremental Multi-Hop in the Lakehouse

19.1. Describe Bronze, Silver, and Gold tables 

19.2. Bronze: what additional metadata could you add for enhanced discoverability?  

19.3. Can you combine streaming and batch workloads in a unified multi-hop pipeline? What about ACID transactions?  

19.4. Describe how you can configure a read on a raw JSON source using Auto Loader with schema inference. What is the cloudFiles.schemaHints option?  

19.5. What happens with the ACID guarantees that Delta Lake brings to your data when you choose to merge this data with other data sources?  

19.6. Describe what happens at the silver level, when we enrich our data.  

19.7. Describe what happens at the Gold level.  

19.8. What is  .trigger(availableNow=True) and when is it used?   

19.9. What are the important considerations for complete output mode with Delta?   

19.10. Describe the two options to incrementally process data, either with a triggered option or a continuous option.  

# 20. Using the Delta Live Tables UI

20.1. Describe how Delta Live Tables makes the ETL lifecycle easier.  

20.2. Beyond transformations, how can you define your data in your code?  

20.3. Describe why large scale ETL is complex when not using DLT.  

20.4. How do you create and run a DLT pipeline in the DLT UI?  

20.6. How do you explore the DAG?  


# 21. SQL for Delta Live Tables

21.1. What is the syntax to do streaming with SQL for Delta Live tables? What's the keyword that shows you're using Delta Live Tables?  

21.2. What is the syntax for declaring a bronze layer table using Auto Loader and DLT?  

21.3. What keyword can you use for quality control? How do you reference DLT Tables/Views and streaming tables?  

21.4. Declaring gold tables.  

21.5. How can you explore the results in the UI?  


# 22. Orchestrating Jobs with Databricks
    
22.1. What is a Job?
    
22.2. When scheduling a Job, what are the two options to configure the cluster where the task runs?

22.3. Running a Job and scheduling a Job  

22.4. How do you repair an unsuccessful job run?  

22.5. How can you view Jobs?  

22.6. How can you view runs for a Job and the details of the runs?  

22.7. How can you export job run results?  

22.8. How do you edit a Job?

22.9. What does Maximum concurrent runs mean?  

22.10. How can you set up alerts? 

22.11. What is Job access control? 

22.12. How do you edit tasks? 

22.13. What are the individual task configuration options? 

22.14. What are the recommendations for cluster configuration for specific job types?  

22.15. What is new with Jobs?  

22.16. Notebook job tips  

# 23. Navigating Databricks SQL and Attaching to Warehouses

23.1. How do you visualise dashboards and insights from your query results?  

23.2. How do you update a DBSQL dashboard?  

23.3. How do you create a new query? 

23.4. How can you set a SQL query refresh schedule?  

23.5. How can you review and refresh your dashboard?  

23.6. How can you share your dashboard?  

23.7. How can you set up an alert for your dashboard?  

23.8. How can you review alert destination options?  

23.9. Can you only use the UI when working with DB SQL?  

# 24. Introducing Unity Catalog

24.1. List the four key functional areas for data governance.  

24.2. Explain how Unity Catalog simplifies this with one tool to cover all of these areas.  

24.3. Walk through a traditional query lifecycle, and how it changes when using Unity Catalog. Highlight the differences and why this makes a query lifecycle much simpler for data consumers.  

# 25. Managing Permissions for Databases, Tables, and Views

25.1. What is the data explorer, how do you access it and what does it allow you to do?  

25.2. What are the default permissions for users and admins in DBSQL?  

25.3. List the 6 objects for which Databricks allows you to configure permissions.  

25.4. For each object owner, describe what they can grant privileges for.  

25.5. Describe all the privileges that can be configured in Data Explorer.  

25.6. Can an owner be set as an individual or a group, or both?  

25.7. What is the command to generate a new database and grant permissions to all users in the DBSQL query editor?
