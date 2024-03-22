---
title : "Create EFS for file systems"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 3.2 </b> "
---

##  Create EFS for file systems

1. File systems settings:
   - Services: **EFS**
   - Choose **Create file systems**
   - Name: **WebServers-EFS-1**
   - Uncheck **Enable automatic backups** (for reduce cost)
   - Transition into infrequent Access (IA): choose **None**
   - Transition into Archive: choose **None**
   - Throught mode: **Bursting**
      
 ![VPC](/images/3-configureefs/321.png?featherlight=false&width=90pc)

 ![VPC](/images/3-configureefs/322.png?featherlight=false&width=90pc)  

 ![VPC](/images/3-configureefs/323.png?featherlight=false&width=90pc)  

 ![VPC](/images/3-configureefs/324.png?featherlight=false&width=90pc)  
 
 ![VPC](/images/3-configureefs/325.png?featherlight=false&width=90pc)  

2. Network access
   - VPC: **WebServers**
   - Mount targets:
     - Remove all default Security groups
     - Configure for Availability zone: **ap-southeast-1a** access to Security group: **WebServers-EFS-1-SG** 
   - Click **Create**
   
 ![VPC](/images/3-configureefs/326.png?featherlight=false&width=90pc)  
 ![VPC](/images/3-configureefs/327.png?featherlight=false&width=90pc)  
 ![VPC](/images/3-configureefs/328.png?featherlight=false&width=90pc)  
 ![VPC](/images/3-configureefs/329.png?featherlight=false&width=90pc)
 ![VPC](/images/3-configureefs/3210.png?featherlight=false&width=90pc)     


3. Checking and copy config EFS via DNS
   - Select **WebServers-EFS-1** VPC
   - Choose **Attach**
   - Choose **COPY** Using the EFS mount helper:
     -  **sudo mount -t efs -o tls fs-0469e4e20cb346954:/ efs**
   
![VPC](/images/3-configureefs/3211.png?featherlight=false&width=90pc) 
![VPC](/images/3-configureefs/3212.png?featherlight=false&width=90pc) 
![VPC](/images/3-configureefs/3213.png?featherlight=false&width=90pc) 
![VPC](/images/3-configureefs/3214.png?featherlight=false&width=90pc) 