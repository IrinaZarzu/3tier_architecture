# AWS_3_tier_web_architecture

![image](https://github.com/IrinaZarzu/3tier_architecture/assets/116802082/9a2e1e91-ec89-42c2-bfb6-37b34400127e)


This repository contains the infrastructure setup for an e-commerce website using a 3-tier architecture on AWS. The setup includes a web application tier, an application tier, and a data tier, ensuring high availability, scalability, and security.
For more information, you can access the blog post [here](https://medium.com/@irinazarzu/aws-3-tier-web-architecture-8310ad0d815a) .

## Project Overview

Our project leverages AWS services to build a robust and secure e-commerce platform. The architecture is designed following the AWS Well-Architected Framework principles, ensuring operational excellence, security, reliability, performance efficiency, cost optimization, and sustainability.

## Architecture Components for an Online Clothing Store.

### Web Application Tier (Presentation Layer)
- **Description**: Handles the user interface and user experience.
- **Example**: Customers browse clothing items, view product details, add items to their cart, and proceed to checkout.

### Application Tier (Business Logic)
- **Description**: Processes core functionalities such as order processing, user authentication, and product catalog management.
- **Example**: Manages logic for adding items to the cart, processing payments, managing user accounts, and updating inventory levels.

### Data Tier (Database)
- **Description**: Securely stores all critical data, such as customer information, transaction records, and product details.
- **Example**: Stores details of each clothing item, customer profiles, order histories, and payment information.

## Key AWS Services Used

- **AWS Systems Manager (SSM)**: Securely connect to EC2 instances without SSH keys or opening additional ports.
- **VPC and Subnets**: Network infrastructure that segregates and secures different layers of the application.
- **Internet Gateway and NAT Gateways**: Manage internet traffic efficiently, ensuring secure and reliable connectivity.
- **Route Tables**: Direct traffic between subnets and gateways.
- **Security Groups**: Control inbound and outbound traffic to the instances.
- **Auto Scaling Groups and Load Balancers**: Ensure high availability and scalability.
- **Amazon RDS**: Provides a managed database with automated backups and multi-AZ deployments.
- **RDS Read Replica**: Enhances performance by offloading read traffic from the primary database.
- **AWS WAF**: Protects the application from common web exploits and vulnerabilities.
- **Amazon CloudFront**: Delivers content efficiently by caching it closer to users.
- **Amazon S3**: Stores important data and backups, securely connected through a VPC Endpoint Gateway.

## Getting Started

### Prerequisites
- AWS IAM Account
- Basic understanding of AWS services

### Setup Steps

1. **Create the VPC and Subnets**: Set up your VPC with public and private subnets.
2. **Configure Route Tables and Gateways**: Set up route tables and associate them with your subnets. Configure Internet Gateway and NAT Gateways.
3. **Set Up Security Groups**: Define security groups to control traffic to your instances.
4. **Launch EC2 Instances**: Deploy instances for the web and application tiers, and set up Auto Scaling Groups and Load Balancers.
5. **Set Up RDS**: Launch an Amazon RDS instance for your database tier.
6. **Configure SSM**: Create an IAM role and use SSM to connect to your EC2 instances securely.
7. **Set Up WAF**: Protect your application using AWS WAF.
8. **Configure CloudFront**: Set up CloudFront to deliver content efficiently.
9. **Connect to S3**: Create an S3 bucket for storing data and connect it through a VPC Endpoint Gateway.

## Conclusion

With this setup, we are ready to handle production workloads. Our architecture can scale, stay secure, offer a smooth user experience, and support sustainability. This project shows the strength of AWS's cloud services and the value of the Well-Architected Framework in designing cloud infrastructure.


