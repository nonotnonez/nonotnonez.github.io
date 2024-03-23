---
title : "Launch Instances and Configure EFS"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 3.3 </b> "
---

## Configuration

**Instances** configure and **Mount EFS** file systems:

   - Select **WebServer1**
   - Connect to Instances
   - In CMD interface run command:
     
     - sudo -i	
     - sudo yum install -y amazon-efs-utils	
     - mkdir data	
     - ls	
     - **sudo mount -t efs -o tls fs-0469e4e20cb346954:/ data**
     - cd data	
     - sudo bash -c "cat >> efs-1-setup.log"	
	   - efs-1 mounted in site A
     - cat efs-1-setup.log	

 ![VPC](/images/3-configureefs/331.png?featherlight=false&width=90pc) 

 ![VPC](/images/3-configureefs/332.png?featherlight=false&width=90pc) 

 ![VPC](/images/3-configureefs/333.png?featherlight=false&width=90pc) 
 
 ![VPC](/images/3-configureefs/334.png?featherlight=false&width=90pc) 


