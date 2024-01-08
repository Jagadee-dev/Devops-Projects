# DevOps-Projects

This repository will have real-time projects using AWS CloudFormation and Terraform as IaC

**Project-1**
Create an Infrastructure for a three-tier application. Where the static content is stored in S3 and served through CDN & Route 53 only.
It's a PHP application, so, create an Elastic-beanstalk environment to deploy my application on multi-container Docker. Also, use Mysql-db to store the dynamic content, and the MySQL instance should be in a cluster. Use AWS Code-Pipeline to manage all builds and deploy. Also, serve the content only from AWS CDN, so please restrict access to serve content through the S3 bucket directly. All the Ec2 instances should be in a private subnet which is not accessible publicly, Only Elastic Load Balancer should be in a Public subnet.

**Steps Involved:**
1) Define the provider and set up the AWS creds.
2) create VPC and subnets
3) create an S3 bucket for storing static content and restrict public access to it.
4) Create a CloudFront distribution for serving content through CDN and Route 53.
5) create MySQL DB cluster.
6) Set up an Elastic Beanstalk application and environment.
7) Create an Elastic Beanstalk application version.
8) create a CI/CD with the AWS Code pipeline
9) Define IAM roles for Code pipeline, Elastic Beanstack, RDS, etc
10) Define security groups for ELB, EC2 Instances, RDS, etc
11) Map the applications Domain name with the help of Route53
