#DAY 6
---

##Virtual Private Cloud (VPC)
---
	It is created at company level.
ISP (Internet Service Providers ) like relience, airtel etc provides sevice through routers.
Router is connected through lease line i.e. wire,
The Internet service provided by Router is used by the customer by LAN connections or by WiFi.

**How to create VPC ?**
---
` services ->VPC ->Isolated Cloud Resources ->VPC ->Create new VPC. `

VPC contains **subnets** they are attached to VPC.
Availablity Zone contains unique subnet each.
**Subnet** contains *Rout Table-* which actully work as router .
It is used to connect with world using *INTERNET GATEWAYS*.
Internet Gateways provide a way to connect to internet.

---


## Cloud Watch & Cloud Trail
---
 
Cloud watch and Cloud trail both are service of AWS .

 
**Cloud Watch**
---

Cloud watch is used to keep watch on *RESOURCES* and *APPLICATIONS*.
Cloud watch database stores all logs 

-Log store.

-Log search(using query).

-You can build dash board on it.

-Can select time frame.


**Cloud Trail**
---

Cloud Trail works as CCTY.
It keeps watch on users *ACTION*.
Users action are stored in cloud trail.
Every second action is get traced in cloud trail.
One can come to know how much time the mchine was idle and how much time the machine is working.

**Status Check**
---
Status check is used to check the backgroung services such as light ,internet etc.
It contains 2/2 status: 

   -Instance properly working.

   -Internet properly working.

**View/Change User Data**
---

Use linux command to edit and update user data if instance is Linux.

user data -> commands -> linux/windows

It always execute as root user ->admin.

You can pass any command or all shell script can be passed depending on which OS you are using.

Feedback commands -> yum update

                   -> yum update -y [y stands for yes]
  
store -> Nav/lib/cloud/instances

---

**Serverless [Lambda]**
---
 
Lambda-> Function -> Create Function -> Use a blueprint -> blueprint (HelloWorld Node.js) ->Function Name
 ->(dacdemo.node)-> robo makerstudent -> create function.

Lambda  -> 1. event driven automation/programming.
           2. lambda as API/request and Response model 
           3. web services


**Lambda as Event Driven Automation/Programming**
---
1. Write a node.js program in configure in S3 bucket.

2. S3 -> bucket

3. Go in properties -> Event Click -> Add notification ->select all object create events->give event name ->send to [lambda] ->selct node.js function
   ->click event ->read file and save the event  

4. Now open Lambda Function ->Open Confiuration ->Open program you scheduled of node.js and print fun in node.js and just save it do not test

5. Now open S3 Overviews upload any file.
   Now your lambda node.js program gets triggered automatically. 
   Check it into cloud watch logs.




