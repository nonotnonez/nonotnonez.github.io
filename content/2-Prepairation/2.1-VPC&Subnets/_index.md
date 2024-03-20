---
title : "VPC & Subnets"
date :  "`r Sys.Date()`" 
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

## VPC

### Basic Features of Security Group

- **Allow Rules Only:** Only Allow rules can be added; Deny rules cannot be added.

![VPC](/images/2-Prepairation/2.1-vpcsubnets/vpcs.png?featherlight=false&width=90pc)


## Subnets

A Security group rule is created to grant access to traffic entering or leaving an instance. This access can apply to a specific CIDR or to a Security group in the same VPC, or even to a Security group in another VPC connected by peering.

### Components of Security Group Rule

- **Inbound Rules:** These include the source of the traffic and the destination port or port range. The source can be another security group, an IPv4 or IPv6 CIDR range, or an IPv4/IPv6 address.

![VPC](/images/2-Prepairation/2.1-vpcsubnets/subnets.png?featherlight=false&width=90pc)