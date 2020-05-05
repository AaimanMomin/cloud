#DAY 5
---
##IAM ROLE
---
 IAM Role using AWS sdk.
 Outside AWS access using aws cli installing on local laptop/pc.

 **COMMANDS FOR AWS CLI** 
 1. aws --version -> If this command runs then your aws cli is prpperly installed.

 2. aws s3 ls

 3. aws configure

 4. Go to aws educate account and click on account details
    AWS CLI `show`
    
    Click on show button and copy all.
    Now go to user folder and search for credential file and clear all credential file and paste the things copied from aws details.
 
 5. Now go to command prompt 
 
    AWS Access Key Id: <copy paste key id from aws account details>
 
    AWS Secret Access Key: <copy paste secret from the same>
 
    Default Region Name : us-east-1
    
    Default output formate : json

 6. aws s3 ls

 7. It will show that , now local is configured with aws.



##Any application installed from local to EC2 vs from RDS
---
 **EC2:** Suppose MySQL is installed in EC2, is managed by aws , but if you install any application within EC2them it is managed by developer.
          No Scalablity.
          No Turn ON/OFF application. 
          No automatic maintainance.

 **RDS:** MySQL server is fully managed by AWS. It contains automatic scalablity, automatic backup, maintainance and also able to turn ON/OFF the server.


## S3
---
   In s3 bucket everything is an object inside bucket. .ie. folder, file, etc.
   
Object are immutable .i.e object cannot be updated/changed.

So you have to delete and upload the updated one.


##SERVERLESS
---

1. You don't own server.

2. Zero mainatainance.

3. Salablity automatic.


    Suppose you have EC2-Server which takes 4GB memory, 500GB Hard Disk,2 core processor which are charged on running mode.
Even if 100% utilization is not done then also you have to pay full charges of 1005 usage.
     

**LAMBDA FUNCTION**
---
   
   1.No Server.
   
   2.Code storage - No cost

   3.When code in running mode - Cost

    Cost is calculated on usage of `(CPU + RAM) * TIME = CHARGE`.
 
No charges of OS. 
It also contains *scalability* and *parallelization*.
  
**Scalablity**
   
    Scale up and Scale down is automatic.
    
eg: 1. 1GB memory, 2 Core - 30 sec

    2. updated -> 2GB , 1 Core - 10 sec

**Parallelization** 

    On every execution request, if simultaneous 1 million requests occurs **Lambda** will handel every 
    request simultaneously.

   
