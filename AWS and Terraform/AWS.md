# AWS IAM

AWS IAM (Identity and Access Management) is a service provided by Amazon Web Services (AWS) that helps you manage access to your AWS resources. It's like a security system for your AWS account.

With IAM, you can control and define permissions through policies. Policies are written in JSON format and specify what actions are allowed or denied on specific AWS resources. These policies can be attached to IAM entities (users, groups, or roles) to grant or restrict access to AWS services and resources.

In simpler words, IAM provides you Authentication and Authorization. Overall, IAM is an essential component of AWS security, providing granular control over access to your AWS account and resources, reducing the risk of unauthorized access and helping maintain a secure environment.

## Components of IAM

Users: IAM users represent individual people or entities (such as applications or services) that interact with your AWS resources.

Groups: IAM groups are collections of users with similar access requirements. Instead of managing permissions for each user individually, you can assign permissions to groups, making it easier to manage access control. Users can be added or removed from groups as needed.

Roles: IAM roles are used to grant temporary access to AWS resources. Roles are typically used by applications or services that need to access AWS resources on behalf of users or other services.

Policies: IAM policies are JSON documents that define permissions. Policies specify the actions that can be performed on AWS resources and the resources to which the actions apply.



# AWS EC2

EC2 instance is a virtual server in AWS that you can use to run app just like you would on a physical server.

### Why EC2 instance?

1. Scalability
2. Reliability and High Availability
3. Cost Efficiency
4. Security 
5. Flexibility

# Virtual Private Cloud (VPC)

 VPC is like you own private isolated network inside a cloud provider (AWS, GCP, Azure). It helps to define which resources should be public and which should be private. For example, the fronend of a website is kept public for the users to access and the Backend (database) which contains vital information is kept private.


# Security Groups

Security Group is like a virtual firewall for your EC2 instance and other resources like RDS, Lambda, etc. It controls whether one can connect from your instance or not. You can allow specific traffic based on protocol, port and IP. You create security group in VPC and attach it to EC2.

## Terms to remember

1. Inbound Traffic: Traffic coming into a resource
2. Outbound Traffc: Traffic going out from a resource


## Route 53:
Route 53 provides DNS as a service. When you try to access any domain Route 53 intercepts the domain and in the hosted zone Route 53 will look for the DNS records. Route 53 also supports health services on web services.

# AWS CloudWatch
AWS CloudWatch is the gatekeeper for AWS which will help you with monitoring, alerting, reporting and logging. It helps in tracking metrics, analyzing logs, setting alarms, and optimizing performance and cost.

Some use cases are:
- Real-time metrics monitoring

- Alarms and automated alerts

- Log Insights for querying and analysis

- Custom application metrics

- Cost optimization

- Auto scaling based on performance metrics


## AWS S3 Bucket
Main Idea about AWS S3:
- S3 is a scalable storage solution on AWS, catering to individuals and organizations for various data storage needs.
- S3 objects are globally accessible via HTTP, ensuring accessibility from anywhere in the world.
- AWS guarantees high reliability with 99.9999% durability for S3, coupled with default object encryption for enhanced security.
- DevOps engineers can efficiently manage S3 buckets, configuring settings for optimal performance and security.
- AWS S3 offers advantages like high availability, scalability, security, cost-effectiveness, and performance enhancements.
- Security features include encryption, access control, object locking, and access logging for auditing purposes.
- S3 provides various storage classes catering to different needs, balancing cost-effectiveness and access time.
- Bucket permissions and policies allow fine-grained access control, enhancing security for sensitive data in S3 buckets.
