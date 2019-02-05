# Introduction to the AWS Cloud

## Intro
- Cloud computing refers to the on-demand delivery of IT resources and applications via the internet
- Before cloud computing, we had to build data centers based on guessing what our max peaks might be
- With cloud computing, instead of having to design/build data centers, we access the data center and all of its resources via the internet, allowing us to scale up or down based on our actual needs, without having to plan for the worst case scenario
- With AWS cloud we can reduce risks, automatically scale our computing to meet our needs, secure our data and ensure coverage even in the face of a natural disaster
  * Reduce risks - cloud computing helps reduce risk by being agile, lowering the cost of change
  * Scalability - the ability to resize your resources as necessary. 
  * Reliability - amazons data centers are hosted all over the world in aws regions. Each region is a separate geographic area that has multiple locations known as availability zones. AZ's consists of one or more discreet data centers with each redundant power, networking and connectivity housed in separate facilities. Allows you to host instances in multiple locations.
  * Security of customer data - Data centers are highly secure staffed 24/7 by security guards
- AWS cloud offers computing, storage, databases, analytics, mobile, networking iot, security and enterprise applications

## Intro to AWS Management Interfaces
- Three ways to use AWS. All three are based on a common API that serves as the foundation for AWS
  1. AWS management console
  2. Command Line Interface (CLI)
  3. Software development kits
- AWS Management Console
  * GUI that allows you to browse through all AWS services
- Command Line Interface
  * Programming language agnostic
  * Open source tool built for interacting with AWS
- Software Development Kits
  * The SDK's enable applications built on AWS to manage your "infrastructure as code"

# Core Services
## Amazon Elastic Cloud Compute (EC2)
- Compute refers to the server resources that are being presented
- Cloud refers to the fact that these are cloud hosted compute resources
- Elastic refers to the fact that, if properly configured, you can increase or decrease the amount of service required by an application automatically according to the current demands on that application
- Amazon refers to the servers as Amazon EC2 instances

## Amazon Elastic Block Store (EBS)
- Block storage is data storage typically used in storage-area network (SAN) environments where data is stored in volumes, aka blocks. Each block is assigned an arbitrary identifier by which it can be stored and retrieved. Each block acts as an individual hard drive.  
- EBS volumes can be used as the storage unit for EC2 instances
- These volumes can be HDD or SDD 

## Amazon Simple Storage Service (S3)
- Amazon S3 is a fully managed cloud storage service that provides a simple API for storing and retrieving data. This means that the data you store in S3 isn't associated with any particular server and you don't have to manage any infrastructure yourself
- Store unlimited number of objects such as images
- In S3 you create buckets to hold your data
- When you create a bucket in S3, its associated with a particular AWS region. Whenever you store data in the bucket, it is redundantly stored across mutliple AWS facilities within your selected region
- If you want to put an object (such as video) into a bucket you need to specify a key which is just a string that can be used to retrieve the object later. Commonly this string resembles a file path
- Access S3 through the management console, the CLI or the SDK's
- Use cases
  * Storing application assets
  * Static web hosting
  * Backup and disaster recovery - good candidate to store backups of your data
  * Staging area for big data

## AWS Global Infrastructure
AWS's global infrastructure can be broken down into 3 topics
1. AWS Regions
  * Regions are geographic areas that host 2 or more availability zones
  * Regions are completely separate from each other
2. Availability Zones
  * AZ's are a collection of data centers in a specific region. Each AZ is physically isolated from the others but connected together by a fast, low-latency network.
3. Edge Locations
  * EL's host a content delivery network or CDN, called Amazon Cloud Front. Cloud Front is used to deliver content to your customers. Requests for content are auto routed to the nearest edge location so that the content is delivered faster to the end users.

## Amazon Virtual Private Cloud (VPC)
- The AWS cloud offers on-demand, pay-as-you-go compute as well as managed services
- It is a networking service
- It is a private, virtual network in the AWS cloud, uses same concepts as on premise networking
- Allows complete control of network configuration
- Offers several layers of security controls including the ability to allow and deny specific internet and internal traffice 

## Security Groups
- Security groups act as built-in firewalls for your virtual servers

# Integrated Services
## Application Load Balancer
- 
## Auto Scaling
## Amazon Route 53
## Amazon Relational Database Services (RDS)
## AWS Lambda
## AWS Elastic Beanstalk
## Amazon Simple Notification Service (SNS)
## Amazon CloudWatch

