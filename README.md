# Notes-7-Storage-

“Cloud storage is typically more reliable, scalable, and secure than traditional on-premises storage system. It holds the information that applications use such as big data analytics, data warehouses, databases, and backup and archive applications all rely on some form of data storage architecture.” 

## Amazon Elastic Block Store (EBS) 

•	Provides block storage volumes for Amazon EC2 instances. (Data storage device that retains data after power is shut off) 

•	Automatically replicated within its availability zone to protect from component failure

•	Provides low latency and durability performance needed to run workloads

•	Scale usage up or down in minutes while keeping low pricing 

•	Benefit of block storage allows user to change on blocks that contain the character needed to change compared to object storage where user must change entire file 

•	User has access to snapshots, encryption, and elasticity of capacity

## Amazon Simple Storage Service (S3)

•	Object-level storage- if you want to change a part of a file, user must make change and reupload entire file again 

•	Data is stored in buckets 

•	Provides 11 9’s of durability and unlimited amounts of objects can be stored into a bucket 

•	No need to manage infrastructure 

•	Fine-grained control on data access through AWS identity

•	Event notifications available along with encryptions

•	Object level storage classes range from: 

    o	Amazon S3 Standard

    o	Amazon S3 Intelligent-Tiering 

    o	Amazon S3 Standard-Infrequent Access 

    o	Amazon S3 One Zone-Infrequent Access 

    o	Amazon S3 Glacier Deep Archive 

•	Pay only for what you use 

•	Price by amount of object in storage, number of requests (Get,Put,Copy), and data transfer

## Amazon Elastic File System (EFS)

•	Implement storage for instances in EC2 that can be accessed by multiple virtual machines at the same time 

•	Build a file system for data and analytics, media workflow, content management, web serving, and home directories

•	File system is supported by strong consistency and file locking 

•	Scale automatically from gigabytes to petabytes of data without provision storage 

## Amazon S3 Glacier 

•	Secure, durable, affordable cloud storage service 

•	Data archiving and long-term backup 

•	Archive is any object like a photo, video, or file stored in the service 


•	Vault is a container for storing archives (access policies and vault lock policies)

•	Retrieval options 

    o	Standard 3-5 hours

    o	Bulk 5-12 hours

    o	Expedited 1-5 minutes 

•	By default, only owner can access data 

“By default, data in Amazon S3 is stored redundantly across multiple facilities. Amazon S3 holds trillions of objects and regularly peaks at millions of requests per second. “ 
