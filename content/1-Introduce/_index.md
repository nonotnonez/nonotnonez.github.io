---
title : "Introduction"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

## Introduction to Amazon EFS

Amazon EFS create a shared storage file system that is available concurrently to multiple instances in Amazon Elastic Compute Cloud (Amazon EC2).

Amazon EFS can be used to share file data without provisioning or managing servers. Amazone EFS automatically grows and shinks as files are added and removed , so capacity doesn't need to me managed. Servers access shared data in Amazon EFS by using mount targets in each Availability Zone.

Applications on each server view each mounted file systems as a local path, similar to "/mnt/efs".

In the following sections, we will: 
- Launch and configure Amazon EFS file system.
- Mount the file system to an Amazon EC2 instance.
- Connect a second EC2 instance to the same file system.
- Share files between the two EC2 instances.