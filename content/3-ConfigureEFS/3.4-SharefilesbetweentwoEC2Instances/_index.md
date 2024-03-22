---
title : "Share files between two EC2 Instance"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 3.4 </b> "
---

##  Setting EFS in diffirent Instane

1. In the **EFS** interface:

   - Select **WebServers-EFS-1-SG**
   - Click **Network** tab
   - Click **Manage**
   - Add mount target:
      - Configure for Availability zone: **ap-southeast-1b** access to Security group: **WebServers-EFS-1-SG** 
 
  ![VPC](/images/3-configureefs/341.png?featherlight=false&width=90pc)
  ![VPC](/images/3-configureefs/342.png?featherlight=false&width=90pc) 
  ![VPC](/images/3-configureefs/343.png?featherlight=false&width=90pc) 
  ![VPC](/images/3-configureefs/344.png?featherlight=false&width=90pc) 
   


2. Checking EFS config:

   ![VPC](/images/3-configureefs/345.png?featherlight=false&width=90pc) 


3. **Instances** configure and **Mount EFS** file systems:
- Select **WebServer2**
   - Connect to Instances
   - In CMD interface run command:
     
     - sudo -i	
     - sudo yum install -y amazon-efs-utils	
     - mkdir data	
     - ls	
     - **sudo mount -t efs -o tls fs-0469e4e20cb346954:/ data**
     - cd data	
     - sudo bash -c "cat >> efs-1-setup.log"	
	   - efs-1 mounted in site B
     - cat efs-1-setup.log	

 ![VPC](/images/3-configureefs/346.png?featherlight=false&width=90pc) 
 ![VPC](/images/3-configureefs/347.png?featherlight=false&width=90pc) 
 ![VPC](/images/3-configureefs/348.png?featherlight=false&width=90pc) 


- We will see data in different Instances
