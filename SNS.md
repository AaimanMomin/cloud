# Day 7
---


##SNS (Simple Notification Service)
---
It is one of the service from AWS services.
When you upload some file in bucket , you should get email.
Here SNS sends notification on email, message, etc.

**How to create SNS ?**

Services->SNS->Topic Name->Next step->Display Name->Access properties->Everyone in both->Create IAM role->
Attach IAM role->Create Topic.

SNS contains two models ,they are *sub and pub model*.

Where *sub* stands for *subscriber* and *pub* stands for *publisher*.
Publisher is where we upload file or folder on which email gets sent to subscriber. The file or data is sent through 
channel called as SNS Channel.Subscriber recives the mail when the file or data is uploaded.

**Create subscription**

Create subscription->Protocol(Email)->endpoint(youremail@gmail.com)->Create subscription.

**Select Publisher**
 
Select publisher and configure SNS Channel to it. 


---


##Snapshot And AMI
---

1. Most important basic difference between AIM's and snapshots are the types of services they are associated with .
   Snapshots are associated with EBS while AIM's are associated wit EC2 instance.

2. Snapshots are the backups of the data on EBS volume, whereas AIM's are bootable copy of the whole EC2 instances.

3. AIM's are used to store the current instance configuration.You can create AIM of instance in stoped status also.

4. When you create a snapshot for an EBS volume that serves as a root device, you should stop the instance befor taking 
   the snapshot.You cannot create snapshots from instances for which hibernation is enable. You cannot create snapshot 
   from hibernated instances.

5. Taking snapshot of non EBS backed instances are not possible but AMI of a non EBS backed instances can be created.

---

##S3 Service
---

S3 contains two categories :
 
1.Select : You can query directly on file data in csv, json, parquet formate using sql.

2.Version : Keep multiple version of object in the same bucket .(Just you have to enable the version and save).
           
            Version has two options (Hide & Show) you can see all versions using *show*.

---

**Default encryption**
---
   Data gets safe as it gets encrypted. By AES-256 it gets locked. By using AWS KMS you can create a key and your 
data will get encrypted.


**Object Lock**
---
   Object lock can be enabled only when a bucket is created.
If you want that your file should not get deleted in any case, then you enable the object lock.

**Requester Pay**
---
   The person who upload and download data ,should get the bill.
*Enable requester pays*:- Requester will pay for requests and data transfer. While Requester pays is enable anonymus 
                          access to this bucket is disabled.  


