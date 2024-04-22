# Project Name: AWS Dynamic Website Deployment

## Overview

This project aims to deploy a dynamic website on AWS infrastructure using various services to ensure reliability, scalability, and security. The deployment architecture includes configuring a Virtual Private Cloud (VPC), setting up subnets, security groups, load balancing, auto scaling, domain registration, and more.

## Architecture

The deployment architecture consists of the following key components:

1. **Virtual Private Cloud (VPC)**: Configured with public and private subnets spanning two availability zones for enhanced reliability and fault tolerance.

2. **Internet Gateway**: Enables connectivity between the VPC instances and the wider internet.

3. **Security Groups**: Serve as a network firewall mechanism to control inbound and outbound traffic to the instances.

4. **Availability Zones**: Utilized to increase system reliability and fault tolerance by deploying resources across multiple zones.

5. **EC2 Instances**: Web servers hosted within private subnets for enhanced security.

6. **NAT Gateway**: Allows instances in private subnets to access the internet securely.

7. **Application Load Balancer (ALB)**: Distributes web traffic evenly to an Auto Scaling Group of EC2 instances across multiple Availability Zones.

8. **Auto Scaling Group**: Automatically manages EC2 instances to ensure website availability, scalability, fault tolerance, and elasticity.

9. **Certificate Manager**: Used to secure application communications with SSL/TLS certificates.

10. **Simple Notification Service (SNS)**: Configured to alert about activities within the Auto Scaling Group for monitoring and management purposes.

11. **Route 53**: Registered the domain name and set up DNS records for the website.

12. **Amazon S3**: Used for storing application code.

## Repository Contents

The GitHub repository contains the following:

1. **Reference Diagram**: A diagram illustrating the architecture and components used in the deployment.

2. **Deployment Scripts**: Scripts for provisioning and configuring the AWS resources mentioned above.

## Getting Started

To deploy the dynamic website using this project:

1. Clone the GitHub repository.
2. Review the reference diagram to understand the architecture.
3. Follow the deployment scripts and instructions provided to provision the necessary AWS resources.
4. Customize the deployment as per your requirements, such as domain name, instance types, and scaling policies.
5. Test the website functionality and scalability.
6. Monitor the system using SNS alerts and other AWS monitoring tools.
7. Optionally, contribute to the project by providing enhancements or optimizations.
