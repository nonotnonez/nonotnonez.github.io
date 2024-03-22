---
title : "VPC & Subnets"
date :  "`r Sys.Date()`" 
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

### VPC

- **Setings:** We will create a manual VPC with config

    VPC Name:    WebServers
    IPxv CIDR:   10.10.0.0/16

![VPC](/images/2-Prepairation/211.png?featherlight=false&width=90pc)


### Subnets

- **Settings:** We will create two subnets with two different Availability Zone

- Subnet 1:
    Subnet Name:        WebServers-Subnet1
    IPv4 CIDR:          10.10.1.0/24
    Availability Zone:  ap-southeast-1a

- Subnet 2:
- 
    Subnet Name:        WebServers-Subnet2
    IPv4 CIDR:          10.10.2.0/24
    Availability Zone:  ap-southeast-1b



![VPC](/images/2-Prepairation/212.png?featherlight=false&width=90pc)