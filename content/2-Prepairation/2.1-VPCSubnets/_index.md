---
title : "VPC & Subnets"
date :  "`r Sys.Date()`" 
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

### VPC configure

- **An AWS Virtual Private Cloud (VPC)** is a virtual network environment within the Amazon Web Services (AWS) cloud platform. It allows you to create a logically isolated section of the AWS cloud where you can launch AWS resources like EC2 instances, RDS databases, and more.

-   We will create a manual VPC with config.
    -   VPC Name:    **WebServers**
    -   IPv4 CIDR:   **10.10.0.0/16**

![VPC](/images/2-prepairation/211.png?featherlight=false&width=90pc)


### Subnets configure

-  **AWS Subnets** are segmented portions of an Amazon Virtual Private Cloud (VPC) network.
-   They allow you to divide the IP address range of your VPC and organize resources into smaller, manageable groups.
-   We will create two subnets with two different Availability Zone.

- Subnet 1:
    - Subnet Name:        **WebServers-Subnet1**
    - IPv4 CIDR:          **10.10.1.0/24**
    - Availability Zone:  **ap-southeast-1a**

- Subnet 2:
    - Subnet Name:        **WebServers-Subnet2**
    - IPv4 CIDR:          **10.10.2.0/24**
    - Availability Zone:  **ap-southeast-1b**



![VPC](/images/2-prepairation/212.png?featherlight=false&width=90pc)