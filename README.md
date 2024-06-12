# Twitter-data-pipeline-using-airflow
In this project, I have built an ETL pipeline in integration of Apache Airflow using CLoud services in AWS. The data is collected from twitter API and entire coding is written in Python for extracting and transforming the data.

### Data/API: [Twitter_API](https://developer.twitter.com/en/portal/projects/1655596629406146563/apps)

### Architecture_Diagram: [Architecture](https://github.com/SameerPathaan/Twitter-data-pipeline-using-airflow/blob/main/Architecture.png)

### Architecture and Pipeline flow
**Twitter API - Airflow on Amazon EC2 - Amazon S3**

Description: The data is extracted from twitter API and raw data is converted into desired format. Some of the imporant features like number of likes of a user, number of retweets, the text that is tweeted etc and the transformations are applied using python. Then a virtual EC2 instance is created to run the orchestration tool Apache Airflow to execute the process on top of it. A Dag folder is created in Apache Airflow using the command line of the virtual machine running on cloud AWS to get the ETL code and Dag code to exectue the Entire ETL Process. Once the Dag runs, it extracts the data directly from the Twitter API, transforms it desired csv format and load the data into Amazon S3

### Services Used
**Apache Airflow:** Apache Airflow is an open-source platform used to programmatically create, schedule, and monitor workflows. It allows users to define, execute, and manage workflows as code, making it easy to manage complex data pipelines. Airflow offers a web interface for users to monitor and control workflows, as well as a rich library of plugins and integrations that enable users to easily connect with a variety of data sources and services.

**EC2:** Amazon Elastic Compute Cloud (EC2) is a scalable cloud computing service that provides users with secure, resizable compute capacity in the cloud. EC2 instances are virtual machines that can be used to run a variety of applications, from simple web servers to complex big data analytics workloads. Users can choose from a wide range of instance types with varying amounts of CPU, memory, and storage resources, and pay only for what they use.

**S3:** Amazon Simple Storage Service (S3) is a cloud storage service that provides users with highly scalable, durable, and secure object storage. Users can store and retrieve any amount of data from anywhere on the internet, using simple web interfaces or APIs. S3 is designed to be highly available and fault-tolerant, with multiple layers of redundancy to ensure data durability. S3 can be used for a variety of use cases, such as backup and recovery, content distribution, and data archiving.

### Installed Packages:
Pandas, apache-airflow, s3fs, tweepy
