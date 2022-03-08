# AWS

#IAM
- securely
- FREE

## RedShift
## EBS

- [Encrypt EBS](https://cloudacademy.com/blog/how-to-encrypt-an-ebs-volume-the-new-amazon-ebs-encryption/)

## ELB
- AWS Global Accelerator
  - ELB provides load balancing within one Region, AWS Global Accelerator provides traffic management across multiple Regions [...] AWS Global Accelerator complements ELB by extending these capabilities beyond a single AWS Region, allowing you to provision a global interface for your applications in any number of Regions. If you have workloads that cater to a global client base, we recommend that you use AWS Global Accelerator. If you have workloads hosted in a single AWS Region and used by clients in and around the same Region, you can use an Application Load Balancer or Network Load Balancer to manage your resources. https://aws.amazon.com/global-accelerator/faqs/


## EC2
### Auto Scaling
- https://docs.aws.amazon.com/autoscaling/ec2/userguide/schedule_time.html
- [lifecycle hooks](https://docs.aws.amazon.com/autoscaling/ec2/userguide/lifecycle-hooks.html)
- 

## VPN
- [Monitoring VPN tunnels using Amazon CloudWatch](https://docs.aws.amazon.com/vpn/latest/s2svpn/monitoring-cloudwatch-vpn.html)

## RDS
- [Storage Types](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_Storage.html)

- [FAQS](https://aws.amazon.com/ebs/faqs/)
- [Read Replicas](https://aws.amazon.com/rds/features/read-replicas/)
- ACID => RDS & DynamoDB but SQL=> RDS only (DynamoDB is No SQL DB)
## CloudTrail
- [AWS CloudTrail Update – Turn on in All Regions & Use Multiple Trails](https://aws.amazon.com/blogs/aws/aws-cloudtrail-update-turn-on-in-all-regions-use-multiple-trails/)

## S3
- Secure your data using Access Control Lists and Bucket Policies
- S3 Standard
- S3 IA
  - Infrequently Acesssed
  - Rapid Access
  - Lower fee than S3
- S3 One Zone - IA
  - One Zone 
- S3 Intelligent Tiering
- S3 Glacier
  - low-cost storage
  - retrieal times from minutes to hours
- S3 Glacier Deep Archive
  - lowest-cost
  - 12 hours

- S3 Buckets:
  - Can access via Bucket Policies, Access Control List
  - Managed Key SSE-S3

- [SSE-C Server Side Encryption with customer provided keys]
- [KMS Key Management Service](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html)
- Storage
  - Expedited — Expedited retrievals allow you to quickly access your data when occasional urgent requests for a subset of archives are required. For all but the largest archives (250 MB+), data accessed using Expedited retrievals are typically made available within 1–5 minutes. Provisioned Capacity ensures that retrieval capacity for Expedited retrievals is available when you need it. For more information, see Provisioned Capacity.

  - Standard — Standard retrievals allow you to access any of your archives within several hours. Standard retrievals typically complete within 3–5 hours. This is the default option for retrieval requests that do not specify the retrieval option.

  - Bulk — Bulk retrievals are Glacier’s lowest-cost retrieval option, which you can use to retrieve large amounts, even petabytes, of data inexpensively in a day. Bulk retrievals typically complete within 5–12 hours.
- [S3 CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/DownloadDistS3AndCustomOrigins.html)
- [Cross region replication(CRR) or Same region replication(SRR)](https://docs.aws.amazon.com/AmazonS3/latest/dev/replication.html#replication-requirements)
- The file gateway employs a local read/write cache to provide a low-latency access to data for file share clients in the same local area network (LAN) as the file gateway.
Good read - https://d0.awsstatic.com/whitepapers/aws-storage-gateway-file-gateway-for-hybrid-architectures.pdf

- Amazon S3 Standard-Infrequent Access

## Amazon Kinesis
+ Amazon Kinesis Data Firehose is a fully managed service for delivering real-time streaming data to destinations such as Amazon Simple Storage Service (Amazon S3), Amazon Redshift, Amazon Elasticsearch Service (Amazon ES), and Splunk. Kinesis Data Firehose is part of the Kinesis streaming data platform, along with Kinesis Data Streams, Kinesis Video Streams, and Amazon Kinesis Data Analytics. With Kinesis Data Firehose, you don't need to write applications or manage resources. You configure your data producers to send data to Kinesis Data Firehose, and it automatically delivers the data to the destination that you specified. You can also configure Kinesis Data Firehose to transform your data before delivering it

## VPC
- [VPC Flow Logs](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html)
- [Compare NAT gateways and NAT instances](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-comparison.html)
- [VPC endpoints](https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints.html)
# [Network ALC](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)
- You can only create deny rules with network ACLs, it is not possible with security groups.
Network ACLs process rules in order from the lowest numbered rules to the highest until they reach
and allow or deny. The following table describes some of the differences between security groups
and network ACLs
## Lamda
- [ENV variable](https://docs.aws.amazon.com/lambda/latest/dg/env_variables.html)

## [EFS](https://aws.amazon.com/efs/)


## VPC
- [Gateway Endpoint](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-endpoints-s3.html)

## SQS
- The visibility timeout begins when Amazon SQS returns a message. During this time, the consumer processes and deletes the message. However, if the consumer fails before deleting the message and your system doesn't call the DeleteMessage action for that message before the visibility timeout expires, the message becomes visible to other consumers and the message is received again. If a message must be received only once, your consumer should delete it within the duration of the visibility timeout.

- [sqs-visibility-timeout](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-visibility-timeout.html)

## Route53
- Geolocation routing policy – Use when you want to route traffic based on the location of your users. Geoproximity routing policy – Use when you want to route traffic based on the location of your resources and, optionally, shift traffic from resources in one location to resources in another.

