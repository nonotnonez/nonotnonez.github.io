---
title : "Resource Cleanup"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---
## Clean up resources

We will proceed to delete the resources in the following order:

1. Delete Instances
    - Access the Amazon EC2
    - Select **WebServers1** and **WebServers2**
    - Select **Terminate**
      
![Terminate EC2](/images/4/ec21.png?featherlight=false&width=90pc)
![Terminate EC2](/images/4/ec22.png?featherlight=false&width=90pc)

2. Delete Security Groups
    - Access to Security Groups
    - Select **WebServers-EFS-1-SG**
    - Select **delete**
      
![Terminate EC2](/images/4/sg1.png?featherlight=false&width=90pc)
![Terminate EC2](/images/4/sg2.png?featherlight=false&width=90pc)

3. Delete file system
    - Access the Amazon EFS
    - Select **WebServers-EFS-1-SG**.
    - Select **delete**
    - Confirm.
   
![Terminate EC2](/images/4/efs.png?featherlight=false&width=90pc)
![Terminate EC2](/images/4/efs-1.png?featherlight=false&width=90pc)





