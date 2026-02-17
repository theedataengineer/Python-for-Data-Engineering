# Python-for-Data-Engineering
Practical implementation of data pipelines, ETL processes, and big data architectures using Python. Documentation of my journey through "Data Engineering with Python".

Book Author: Paul Crickard

Revised By: Kirimi Dennis

## TABLE OF CONTENTS

### SECTION 1: Building Data Pipelines - Extract, Transform, and Load

#### 1. What is Data Engineering?

- What data engineers do
- Required skills and knowledge to be a data engineer
- Data engineering vs data science
- Data engineering tools
- Programming languages databases
- Database processing engines
- Data pipelines
- Summary

#### 2. Building our Data Engineering Infrastructure

- Installing and configuring Apache NiFi
- A quick tour of NiFi
- PostgreSQL driver
- Installing and configuring Apache Airflow
- Installing and configuring Elasticsearch
- Installing and configuring Kibana
- Installing and configuring PostgreSQL
- Installing PgAdmin 4
- A tour if PgAdmin 4
- Summary

#### 3. Reading and Writing Files

- Writing and reading files in Python
- Writing and reading CSVs
- Reading and writing CSVs using Pandas Dataframes
- Writing JSON with Python
- Building data pipelines in Apache Airflow
- Handling files using NiFi processors
- Working with CSV in NiFi
- Working with JSON in NiFi
- Summary

#### 4. Working with Databases

- Inserting and extracting relational data in python
- Inserting data into PostgreSQL
- Inserting and extracting NoSQL database data in Python
- Installing Elasticsearch
- Inserting data into Elasticsearch
- Building data pipelines in Apache Airflow
- Setting up Airflow boilerplate
- Running the DAG
- Handling databases with NiFi processors
- Extracting data from PostgreSQL 
- Running the data pipeline
- Summary

#### 5. Cleaning, Transforming, and Enriching Data

- Performing exploratory data analysis in python
- Downloading the data
- Basic data exploration
- Handling common data issues using pandas
- Drop rows and columns
- Creating and modifying columns
- Enriching data
- Cleaning data using Airflow
- Summary

#### 6. Building a 311 Data Pipeline

- Building the data pipeline
- Mapping a data type
- Triggering a pipeline
- Querying SeeClickFix
- Transforming the data for Elasticsearch
- Getting every page
- Backfilling data
- Buiding a kibana dashboard
- Creating visualizations
- Creating a dashboard
- Summary

### SECTION 2: Deploying Data Pipelines in Production

#### 7. Features of a Production Pipeline

- Staging and validating data
- Staging data
- Validating data with great expectations
- Building idempotent data
- Pipelines
- Building atomic pipelines
- Summary

#### 8. Version Control with NiFi Registry

- Installing and configuring the NiFi Registry
- Installing the NiFi Registry
- Configuring the NiFi Registry
- Using the Registry in NiFi
- Adding the Registry to NiFi
- Versioning your Data Pipelines
- Using git-persistence with the NiFi Registry
- Summary

#### 9. Monitoring Data Pipelines

- Monitoring NiFi using the GUI
- Monitoring NiFi with the status bar
- Monitoring NiFi with processors
- Using Python with the NiFi REST API
- Summary

#### 10. Deploying Data Pipelines

- Finalizing your data pipelines for production
- Backpressure
- Improving processor groups
- Using the NiFi variable registry
- Deploying your data pipelines
- Using the simplest strategy
- Using the middle strategy
- Using multiple registries
- Summary

#### 11. Building a Production Data Pipeline

- Creating a test and production environment
- Creating the databases
- Populating a data lake
- Building a production data pipeline
- Reading the data lake
- Scanning the data lake
- Inserting the data into staging
- Querying the staging database
- Validatng the staging data
- Insert warehouse
- Deploying a data pipeline in production
- Summary

### SECTION 3: Beyond Batch - Building Real-Time Data Pipelines

#### 12: Building a Kafka Cluster

- Creating ZooKeeper and Kafka clusters
- Downloading Kafka and setting up the environment
- Configuring ZooKeeper and Kafka
- Starting the ZooKeeper and Kafka
- Clusters
- Testing the Kafka cluster
- Testing the cluster with messages
- Summary

#### 13. Streaming Data with Apache Kafka

- Understanding logs
- Understanding how Kafka uses logs
- Topics
- Kafka producers and consumers
- Building data pipelines with Kafka and NiFi
- The Kafka producer
- The Kafka consumer
- Differentiating stream processing from batch processing
- Producing and consuming with Python
- Writing a Kafka producer in Python
- Writing a Kafka consumer in Python
- Summary

#### 14. Data Processing with Apache Spark

- Installing and running Spark
- Installing and configuring PySpark
- Processing data with PySpark
- Spark for data engineering
- Summary

#### 15. Real-Time Edge Data with MiNiFi, Kafka, and Spark

- Setting up MiNiFi
- Building a MiNiFi task in NiFi
- Summary
