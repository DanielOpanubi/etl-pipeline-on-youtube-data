# etl-pipeline-on-youtube-data
Data pipeline to load, transform, store and visualize data in AWS infrastructure

## Architecture Diagram
![Youtube project](https://user-images.githubusercontent.com/99402393/212493704-d06e2feb-8b90-4e31-8bb1-72d74be22074.jpg)

## Project Goals
1. Data Ingestion — Build a mechanism to ingest data from different sources
2. ETL System — We are getting data in raw format, transforming this data into the proper format
3. Data lake — We will be getting data from multiple sources so we need centralized repo to store them
4. Scalability — As the size of our data increases, we need to make sure our system scales with it
5. Cloud — We can’t process vast amounts of data on our local computer so we need to use the cloud, in this case, we will use AWS
6. Reporting — Build a dashboard to get answers to the question we asked earlier

## Tech Stack
1. Python
2. SQL
3. Data Pipeline
4. AWS basics
5. Data engineering basics

Services Used
1. AWS S3: Amazon S3 or Amazon Simple Storage Service is a service offered by Amazon Web Services that provides object storage through a web service interface. We use S3 to store all our data for the project.
2. AWS Glue: AWS Glue is a serverless data integration service that makes it easier to discover, prepare, move, and integrate data from multiple sources for analytics, machine learning (ML), and application development. We make use of crawlers to create databases and tables from data stored in our S3 buckets, and learn to use glue jobs to create or process new databases, tables similar to how crawlers work.
3. QuickSight: Amazon QuickSight is a cloud-native, serverless, business intelligence with native ML integrations and usage-based pricing, allowing insights for all users. We visualize our final dashboard on Quicksight.
4. AWS Lambda: AWS Lambda is a serverless, event-driven compute service that lets you run code for virtually any type of application or backend service without provisioning or managing servers. We preprocess our data for Glue and automate our pipeline with Lambda.
5. AWS Athena: Athena provides a simplified, flexible way to analyze petabytes of data where it lives. Analyze data or build applications from an Amazon Simple Storage Service (S3) data lake and 25-plus data sources, including on-premises data sources or other cloud systems using SQL or Python.
6. AWS IAM: With AWS Identity and Access Management (IAM), you can specify who or what can access services and resources in AWS, centrally manage fine-grained permissions, and analyze access to refine permissions across AWS.


## Dataset Used
This Kaggle dataset contains statistics (CSV files) on daily popular YouTube videos over the course of many months. There are up to 200 trending videos published every day for many locations. The data for each region is in its own file. The video title, channel title, publication time, tags, views, likes and dislikes, description, and comment count are among the items included in the data. A category_id field, which differs by area, is also included in the JSON file linked to the region.

https://www.kaggle.com/datasets/datasnaek/youtube-new

## Video Walkthrough
- Session 1 - Introduction and data ingestation(Unavailable)
- Session 2 - Creating Databases and tables [link](https://drive.google.com/file/d/18TVoPyI5CCnRDFYSBu4yj65zf0ytx9M6/view?usp=share_link)
- Session 3 - Data preprocessing [link](https://drive.google.com/file/d/11l7l-kYuDzk2jIi7L0ezXB0pxWO8mfRA/view?usp=sharing)
- Session 4 - ETL Job and Automation [link](https://www.youtube.com/watch?v=SUqDUas_Pmk)
- Session 5 - Analytics and Visualization [link](https://www.youtube.com/watch?v=lByY7cQcY7o)
