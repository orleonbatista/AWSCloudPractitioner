# AWS Cloud Practitioner - Services

# Analytics

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


KeyWords: Analyze data in S3, Use standard SQL, ServerLess, Can be integrated with the AWS Glue Data Catalog (Store Metadata) and Amazon Quick Sight (Data Visualization), Charges are applied based on the amount of data scanned


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
* Amazon ES launches the Elasticsearch cluster???s resources and 
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

KeyWords: Managed Service, Launches the Elasticsearch cluster???s with a few clicks, Can be integrated with Kibana and Logstash to provide an enhaced search experience

# Amazon EMR

Amazon EMR (Elastic Map Reduce) is a 
service used to process and analyze large 
amounts of data in the cloud using Apache 
Hive, Hadoop, Apache Flink, Spark, etc.

* The main component of EMR is a cluster that collects Amazon EC2 instances 
(also known as nodes in EMR).
* It decouples the compute and storage layer by scaling independently and 
storing cluster data on Amazon S3.
* It also controls network access for the instances by configuring instance 
firewall settings.
* It offers basic functionalities for maintaining clusters such as monitoring, 
replacing failed instances, bug fixes, etc.
* It analyzes machine learning workloads using Apache Spark MLlib and 
TensorFlow, clickstream workloads using Apache Spark and Apache Hive, and 
real-time streaming workloads from Amazon Kinesis using Apache Flink.
* It provides more than one compute instances or containers to process the 
workloads and can be executed on the following AWS services:
  * Amazon EC2 
  * Amazon EKS 
  * AWS Outposts

It offers basic functionalities for maintaining clusters such as

* Replacing failed instances
* Monitoring
* Bug fixes 

KeyWords: Process and analyze large amounts of data, Cluster that collects Amazon EC2 instances, Offers replacing failed instances, monitoring and bug fixes

# Amazon Kinesis Data Streams

Amazon Kinesis Data Streams (KDS) is a 
scalable real-time data streaming service. It 
captures gigabytes of data from sources like 
website clickstreams, events streams 
(database and location-tracking), and social 
media feeds. It an alternative to 
Apache Kafka..

* Kinesis family consists of Kinesis Data Streams, Kinesis 
Data Analytics, Kinesis Data Firehose, and Kinesis Video 
Streams.
* The Real-time data can be fetched from Producers that 
are Kinesis Streams API, Kinesis Producer Library (KPL), 
and Kinesis Agent.
* It allows building custom applications known as Kinesis 
Data Streams applications (Consumers), which reads 
data from a data stream as data records.
* Data Streams are divided into Shards / Partitions whose data 
retention is 1 day (by default) and can be extended to 7 days
* Each shard provides a capacity of 1MB per second input data 
and 2MB per second output data.

KeyWords: Scalable real-time data streaming service, An alternative to Apache Kafka 

# Amazon Kinesis Data Firehose

Amazon Kinesis Data Firehose is a serverless
service used to capture, transform, and load 
streaming data into data stores and analytics 
services.

* It synchronously replicates data across three AZs while 
delivering them to the destinations.
* It allows real-time analysis with existing business intelligence 
tools and helps to transform, batch, compress and encrypt 
the data before delivering it.
* It creates a Kinesis Data Firehose delivery stream to send 
data. Each delivery stream keeps data records for one day. 
* It has 60 seconds minimum latency or a minimum of 32 MB 
of data transfer at a time.
* Kinesis Data Streams, CloudWatch events can be considered 
as the source(s) to Kinesis Data Firehose.

It delivers streaming data to the following services:

* Amazon S3
* Splunk
* Amazon Redshift
* Amazon Elasticsearch Service

KeyWords: ServerLess, Real-time analysis with existing business intelligence tools, capture, transform, and load streaming data

# Amazon Managed Streaming for Apache Kafka

Amazon Managed Streaming for Apache Kafka 
(Amazon MSK) is a managed cluster service 
used to build and execute Apache Kafka 
applications for processing streaming data.

It helps to populate machine learning 
applications, analytical applications, 
data lakes, and stream changes to and 
from databases using Apache Kafka 
APIs

It provides multiple kinds of security 
for Apache Kafka clusters, including:

* Encryption at Rest 
* AWS IAM for API Authorization
* Apache Kafka Access Control Lists (ACLs)

It easily configures applications by removing all the 
manual tasks used to configure. 

The steps which Amazon MSK manages are:
* Replacing servers during failures
* Handling server patches and upgrades with no downtime
* Maintenance of Apache Kafka clusters
* Maintenance of Apache ZooKeeper
* Multi-AZ replication for Apache Kafka clusters
* Planning scaling events

Amazon MSK Integrates with:

* AWS Glue: To execute Apache Spark job on Amazon MSK cluster
* Amazon Kinesis Data Analytics: To execute Apache 
Flink job on Amazon MSK cluster
* Lambda Functions

KeyWords: Managed Service, Cluster, Helps to populate, Multiple kinds of security

# Amazon Redshift

Amazon Redshift is a fast and petabyte-scale, 
SQL based data warehouse service used to 
analyze data easily

Functions of Redshift:
* It supports Online Analytical Processing (OLAP) type of DB 
workloads and analyzes them using standard SQL and existing 
Business Intelligence (BI) tools (AWS QuickSight or Tableau).
* It is used for executing complex analytic queries on semi-structured 
and structured data using query optimization, columnar-based 
storage, and Massively Parallel Query Execution (MPP).
* Redshift Spectrum helps to directly query from the objects (files) 
on S3 without actually loading them.
* It has the capability to automatically copy snapshots (automated 
or manual) of a cluster to another AWS Region

Pricing details:
* It offers on-demand pricing that will charge by the hour with 
no commitments and no upfront costs.
* Charges are applied based on the type and number of nodes 
used in the Redshift Cluster.
* Charged based on the number of bytes scanned by Redshift 
Spectrum, rounded up to 10MB minimum per query.

KeyWords: Petabyte-scale, SQL based, data warehouse

# AWS Glue

AWS Glue is a serverless ETL (extract, 
transform, and load) service used to 
categorize data and move them between 
various data stores and streams.

Properties of AWS Glue:

* It has a central repository known as the AWS Glue Data Catalog 
that automatically generates Python or Scala code.
* It processes semi-structured data using a simple ???dynamic??? frame in 
the ETL scripts similar to an Apache Spark data frame that organizes 
data into rows and columns.
* It allows organizations to work together and perform data 
integration tasks, like extraction, normalization, combining, loading, 
and running ETL workloads. 
* It supports data integration, preparing and combining data for 
analytics, machine learning, and other applications??? development.
* It helps execute the Apache Spark environment???s ETL jobs by 
discovering data and storing the associated metadata in the AWS Glue 
Data Catalog.
* AWS Glue and Spark can be used together by converting dynamic 
frames and Spark data frames to perform all kinds of analysis.

AWS Glue works with the following services:
* Redshift - for data warehouses
* S3 - for data lakes
* RDS or EC2 instances - for data stores

KeyWords: ServerLess, ETL, central repository, data integration tasks

# AWS Lake Formation

AWS Lake Formation is a cloud service that 
is used to create, manage and secure data 
lakes. It automates the complex manual 
steps required to create data lakes.

A data lake is a secure repository that 
stores all the data in its original form 
and is used for analysis.

* Lake Formation is pointed at the data sources, then crawls 
the sources and moves the data into the new Amazon S3 data 
lake.
*  It integrates with AWS Identity and Access Management 
(IAM) to provide fine-grained access to the data stored in 
data lakes using a simple grant/revoke process

AWS Lake Formation integrates with:
* Amazon CloudTrail
* Amazon CloudWatch
* Amazon EMR
* Amazon Glue: Both use same Data Catalog
* AWS Key Management Service
* Amazon Redshift Spectrum
* Amazon Athena: Athena's users can query those AWS Glue 
catalog which has Lake Formation permissions on them.

KeyWords: Data Lake, secure repository, original form

# Application Integration

# AWS Step Functions
