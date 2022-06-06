# Big-Data-Project

# Batch Processing using AWS EMR & Pyspark
AWS services: S3 as storage,
EMR as processing cluster, and Athena for querying the processed results.
# Business Overview:
In a professional data engineering career, we encounter various scenarios where data gets
collected every day. The data can be processed once a day, i.e., batch processed, and the
processed results are stored in a location to derive insights and take appropriate action based
on the insights. In this project,I try to implement this using AWS services. I
will take a day’s worth of data related to Wikipedia, and perform batch processing on
it.
# Data Pipeline:
The sample data will be put into a folder in the S3 bucket, and run
PySpark code that will run on the EMR cluster. This code will fetch the data from the S3
bucket, perform filtering and aggregation on this data, and push the processed data back into
S3 in another folder. I will then use Athena to query this processed data present in S3. I
will create a table on top of the processed data by providing the relevant schema and then use
ANSI SQL to query the data.
# Agenda:
Explore the services that will be used in this project
Understand the problem statement and look into the architecture used to solve the problem statement.
Set up the AWS services that will be used. 
Write the PySpark code, which will perform batch processing. 
Try to run this code on the EMR cluster. 
# Goal:
To see if I have  the desired output in the desired S3 location. Then, in
AWS Athena, create the tables corresponding to the processed data and use
these tables to query the processed data present in S3.

# Teckstack
Languages - Python
Package - Pyspark
Services - AWS EMR, AWS S3, AWS Athena.
# Amazon S3
Amazon S3 is an object storage service that provides instant scalability, data availability,
security, and performance. Users can save and retrieve any amount of data using Amazon S3,
irrespective of time and location. AWS charges the user per GB of data stored. It also
provides features to customize different roles for accessing the data for various organizational
requirements.
# Amazon EMR
Amazon EMR (Elastic MapReduce) is an AWS tool for big data processing and analysis. It
processes big data across a Hadoop cluster of virtual servers on Amazon Elastic Compute
Cloud (EC2) and Amazon Simple Storage Service (S3). The user can set up a hassle cluster
in a few minutes.
# Amazon Athena
Amazon Athena is an interactive query service that uses standard SQL to query data and
analyze big data in Amazon S3. Under the hood, it uses Presto, a distributed SQL engine, to
run queries. We can query structured, semi-structured, and unstructured data types that might
be stored in formats like CSV, AVRO, Parquet, etc. Athena is server-less, so there is no
infrastructure to set up or manage, and you pay only for the queries you run.
# My Key Takeaways from this project:
◦ Understanding the project overview
◦ Understanding the problem statement
◦ Understanding the project architecture
◦ Creating EC2 key-pair
◦ Creating AWS EMR Cluster
◦ Creating AWS S3 buckets and folders
◦ Uploading JSON data files to AWS S3
◦ Developing and executing the transformation & actions on data
◦ Performing data analysis using AWS Athena
