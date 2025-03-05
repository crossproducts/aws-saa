<div align="center">
    <h1>AWS Solution Architect Associate</h1>
    <h1>CAO-03</h1>
    <h1>Study Guide</h1>
</div>

---

## Content Outline:
The exam has the following content domains and weightings: 
* Domain 1: Design Secure Architectures (30% of scored content) 
* Domain 2: Design Resilient Architectures (26% of scored content) 
* Domain 3: Design High-Performing Architectures (24% of scored content) 
* Domain 4: Design Cost-Optimized Architectures (20% of scored content) 

---

<!--
>> <details close>
>> <summary><h5></h5></summary>
>> <br>
>> </details>
-->

## AWS Services and Features:

### Analytics:

> #### Data Processing:
>> <details close>
>> <summary><h5>Amazon EMR</h5></summary>
>> <br>
>> </details>

>> <details close>
>> <summary><h5>AWS Glue</h5></summary>
>> <br>
>> </details>

>> <details close>
>> <summary><h5>AWS Data Pipeline</h5></summary>
>> <br>
>> </details>

> #### Data Streaming:
>> <details close>
>> <summary><h5>Amazon Kinesis</h5></summary>
>> <br>
>> </details>

>> <details close>
>> <summary><h5>Amazon Managed Streaming for Apache Kafka (Amazon MSK)</h5></summary>
>> <br>
>> </details>

> #### Data Storage & Querying
>> <details close>
>> <summary><h5>Amazon Athena</h5></summary>
>> <br>
>> 📝 Definition: A serverless interactive query service that allows users to analyze data in Amazon S3 using standard SQL.  <br>
>> 💡 Use Case: Ad hoc querying of structured and unstructured data stored in S3.   <br>
>> 🔑 Key Feature: No infrastructure to manage; pay-per-query pricing.  <br>
>> ✅ Tip: Remember that Athena queries data directly from S3 using SQL, making it a cost-effective alternative to a traditional data warehouse.  <br>
>> </details>

##### Amazon Redshift
##### Amazon OpenSearch Service
##### AWS Lake Formation
#### Analytics: Data Visualization & Reporting:
##### Amazon QuickSight
#### Analytics: Data Integration w/ Third-Party Data:
##### AWS Data Exchange
#### Analytics: Compare Similar Services:
##### Kinesis vs. MSK → Kinesis is AWS-native; MSK is for Kafka users.
##### Athena vs. Redshift → Athena is serverless for ad-hoc queries; Redshift is a data warehouse for structured data.
##### Glue vs. Data Pipeline → Glue is serverless and automated; Data Pipeline gives more control.
#### Analytics: Exam Quick Wins:


### Application Integration:
• Amazon AppFlow
• AWS AppSync
• Amazon EventBridge
• Amazon MQ
• Amazon Simple Notification Service (Amazon SNS)
• Amazon Simple Queue Service (Amazon SQS)
• AWS Step Functions
Compare Similar Services:
Exam Quick Wins:

### AWS Cost Management:
• AWS Budgets
• AWS Cost and Usage Report
• AWS Cost Explorer
• Savings Plans

### Compute:
• AWS Batch
• Amazon EC2
• Amazon EC2 Auto Scaling
• AWS Elastic Beanstalk
• AWS Outposts
• AWS Serverless Application Repository
• VMware Cloud on AWS
• AWS Wavelength

### Containers:
• Amazon ECS Anywhere
• Amazon EKS Anywhere
• Amazon EKS Distro
• Amazon Elastic Container Registry (Amazon ECR)
• Amazon Elastic Container Service (Amazon ECS)
• Amazon Elastic Kubernetes Service (Amazon EKS)

### Database:
• Amazon Aurora
• Amazon Aurora Serverless
• Amazon DocumentDB (with MongoDB compatibility)
• Amazon DynamoDB
• Amazon ElastiCache
• Amazon Keyspaces (for Apache Cassandra)
• Amazon Neptune
• Amazon Quantum Ledger Database (Amazon QLDB)
• Amazon RDS
• Amazon Redshift

### Developer Tools:
• AWS X-Ray

### Front-End Web and Mobile:
• AWS Amplify
• Amazon API Gateway
• AWS Device Farm
• Amazon Pinpoint

### Machine Learning:
• Amazon Comprehend
• Amazon Forecast
• Amazon Fraud Detector
• Amazon Kendra
• Amazon Lex
• Amazon Polly
• Amazon Rekognition
• Amazon SageMaker
• Amazon Textract
• Amazon Transcribe
• Amazon Translate


### Management and Governance:
• AWS Auto Scaling
• AWS CloudFormation
• AWS CloudTrail
• Amazon CloudWatch
• AWS Command Line Interface (AWS CLI)
• AWS Compute Optimizer
• AWS Config
• AWS Control Tower
• AWS Health Dashboard
• AWS License Manager
• Amazon Managed Grafana
• Amazon Managed Service for Prometheus
• AWS Management Console
• AWS Organizations
• AWS Proton
• AWS Service Catalog
• AWS Systems Manager
• AWS Trusted Advisor
• AWS Well-Architected Tool

### Media Services:
• Amazon Elastic Transcoder
• Amazon Kinesis Video Streams

### Migration and Transfer:
• AWS Application Discovery Service
• AWS Application Migration Service
• AWS Database Migration Service (AWS DMS)
• AWS DataSync
• AWS Migration Hub
• AWS Snow Family
• AWS Transfer Family

### Networking and Content Delivery:
• AWS Client VPN
• Amazon CloudFront
• AWS Direct Connect
• Elastic Load Balancing (ELB)
• AWS Global Accelerator
• AWS PrivateLink
• Amazon Route 53
• AWS Site-to-Site VPN
• AWS Transit Gateway
• Amazon VPC

### Security, Identity, and Compliance:
• AWS Artifact
• AWS Audit Manager
• AWS Certificate Manager (ACM)
• AWS CloudHSM
• Amazon Cognito
• Amazon Detective
• AWS Directory Service
• AWS Firewall Manager
• Amazon GuardDuty
• AWS IAM Identity Center (AWS Single Sign-On)
• AWS Identity and Access Management (IAM)
• Amazon Inspector
• AWS Key Management Service (AWS KMS)
• Amazon Macie
• AWS Network Firewall
• AWS Resource Access Manager (AWS RAM)
• AWS Secrets Manager
• AWS Security Hub
• AWS Shield
• AWS WAF

### Serverless:
• AWS AppSync
• AWS Fargate
• AWS Lambda

### Storage:
• AWS Backup
• Amazon Elastic Block Store (Amazon EBS)
• Amazon Elastic File System (Amazon EFS)
• Amazon FSx (for all types)
• Amazon S3
• Amazon S3 Glacier
• AWS Storage Gatewa










### Types of Storage:


1. Block Storage (EBS, Instance Store)
Structure: Data is stored in fixed-sized blocks and managed at the block level.
Access: Low-latency access via attached storage to an instance (like a hard drive or SSD).
Use Case: Ideal for databases, virtual machines, and applications requiring frequent read/write operations.
Examples:
Amazon EBS (Elastic Block Store) – Persistent storage for EC2 instances.
Instance Store – Ephemeral storage directly attached to EC2 instances.
2. File Storage (EFS, FSx)
Structure: Data is stored in a hierarchical directory structure (like a traditional file system).
Access: Multiple instances/clients can access the same shared storage using file protocols (NFS, SMB).
Use Case: Ideal for shared storage across multiple applications, containerized workloads, and analytics.
Examples:
Amazon EFS (Elastic File System) – A fully managed NFS file system for Linux workloads.
Amazon FSx – Fully managed file systems, including:
FSx for Windows File Server – SMB file shares for Windows workloads.
FSx for Lustre – High-performance file storage for HPC and ML.
3. Object Storage (S3, Glacier)
Structure: Data is stored as objects with metadata and a unique identifier in a flat namespace.
Access: Accessed via API over HTTP(S), optimized for high durability and scalability.
Use Case: Best for storing large amounts of unstructured data, such as backups, media files, logs, and machine learning datasets.
Examples:
Amazon S3 (Simple Storage Service) – Highly scalable and durable storage.
Amazon Glacier – Low-cost, long-term archival storage.




## References:
Me lol
SAA-C03 AWS Certified Solutions Architect Practice Exam Question and Answers | Practice SAA-C03
https://aws.amazon.com/certification/certified-solutions-architect-associate/
AWS-Certified-Solutions-Architect-Associate_Exam-Guide.pdf

