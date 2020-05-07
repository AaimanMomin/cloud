#DAY 8
 ---

##CFT (Cloud Formation Template)
---

	CFT Creates and Manages Resources with Template.

It is used for one click automation .
It works inside cloude for AWS.
You can use Cloud Formation Template to avoid step wise formation of instances of resources.
CFT is in JSON formate.

**Template**-> Region wise samples of template are given by AWS.



#Important aspects in CFT JSON
---

1. **Parameter**

       * Parameters are like function argument. They are called as CFT Paremeters.

       * Parameters are used to make the code dynamic.

       * Gving parameters is optional.

2. **Resources**

       * EC2, Lambda, etc are resources.

       * Giving resources in CFT is manditory.

3. **Output**

       * Print Public IP.

       * Giving output is optional. 



**CFT creation**
---

CloudFormation->Stack->Create Stack->Template is ready->Specify template ->Uploade a template file->
Choose File-> CFT(file select->open)->Next->Stack name(Give name)->Parameters->(t2-micro)->key name
(give your key name)->security group->subnet->VPC->Next-> Tags(Name:CFT-EC2)->Next->cCreate instance.


**Benifits of CFT**
---

If we write one CFT and create so many resources in it like EC2, Lambda, S3 bucket, snapshot, RDS, IAM Role.
Deleting CFT will delete all the resources above.
The resources made on CFT gets all deleted when we delete the CFT.