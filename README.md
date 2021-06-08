# AWS Cloud Practitioner

# Amazon Athena

Amazon Athena is an interactive serverless 
service used to analyze data directly in 
Amazon Simple Storage Service using 
standard SQL ad-hoc queries.

* Using Athena, ad-hoc queries can be executed using ANSI SQL 
without actually loading the data into Athena.
* It can be integrated with Amazon Quick Sight for data visualization 
and helps to generate reports with business intelligence tools.
* It executes multiple queries in parallel, so no need to worry about 
compute resources.
* It helps to analyze different kinds of data (unstructured, semi-structured, and structured) stored in Amazon S3. 
* It can be integrated with the AWS Glue Data Catalog to store metadata 
in Amazon S3 and offers data discovery features of AWS Glue.
* It helps to connect SQL clients with a JDBC or an ODBC driver. 
* It supports various standard data formats, such as CSV, JSON, ORC, 
Avro, and Parquet. 

Pricing details:

* Charges are applied based on the amount of data scanned by 
each query at standard S3 rates for storage, requests, and data 
transfer. 
* Canceled queries are charged based on the amount of data 
scanned.
* No charges are applied for Data Definition Language (DDL) 
statements.
* Charges are applied for canceled queries also based on the 
amount of data scanned.
* Additional costs can be reduced if data gets compressed, 
partitioned, or converted into a columnar format.


KeyWords: Analyze data in S3, Use standard SQL, ServerLess, Can be integrated with the AWS Glue Data Catalog (Store Metadata) and Amazon Quick Sight (Data Visualization), Charges are applied based on the amount of data scanned.

# Amazon Elasticsearch Service

Amazon Elasticsearch Service (Amazon ES) is a 
managed service that allows users to deploy, 
manage, and scale Elasticsearch clusters in 
the AWS Cloud. Amazon ES provides direct 
access to the Elasticsearch APIs.

Elasticsearch is a free and open-source search
engine for all types of data like textual, 
numerical, geospatial, structured, and 
unstructured.

* Amazon ES with Kibana (visualization) & Logstash (log 
ingestion) provides an enhanced search experience for the 
applications and websites to find relevant data quickly. 
* Amazon ES launches the Elasticsearch cluster’s resources and 
detects the failed Elasticsearch nodes and replaces them.
* The Elasticsearch cluster can be scaled with a few clicks in 
the console

Can be integrated with the following services:
* Amazon CloudWatch
* Amazon CloudTrail
* AWS IAM
* Amazon Kinesis
* AWS Lambda
* Amazon S3
* Amazon ES
* Amazon DynamoDB

Pricing details:
* Charges are applied for each hour of use of EC2 instances and storage volumes attached to the instances.
* Amazon ES does not charge for data transfer between availability zones.

KeyWords: 
