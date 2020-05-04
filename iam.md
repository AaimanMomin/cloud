#IAM ROLES

---

 IAM stands for *Identity Access Management*.

Coummination betwwen the services in AWS is not allowed by default. 
There are may ways to create communication between the AWS services.

1.aws li (linux)

2sdk (java , python, c#, node.js)

IAM Role contains the Policies which are created and attached to IAM Role and this IAM Roles are attached to 
ec2, which allows the communication between ec2 and s3 bucket or other service.

 IAM Roles is secure way to grant permission to entities that you trust.
Example  entities includes the following
 
* IAM user in another account.

* Application code running on an EC2 instance that needs to perform action on AWS resources.

* An AWS service that needs to act on resources in your account to provide the features.

* User from a computer directory who use identity federation with SAMI.

IAM Role issue key that are valid for short duration, making them a more secure to grant access.
