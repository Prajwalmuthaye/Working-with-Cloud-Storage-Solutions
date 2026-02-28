# Working with Cloud Storage Solutions (AWS)

This project demonstrates hands-on experience with different cloud storage services provided by Amazon Web Services (AWS). The objective was to understand the working, characteristics, and use cases of:

>Object Storage
>Block Storage
>File Storage

The services explored include:

>Amazon S3
>Amazon Elastic Block Store
>Amazon Elastic File System

# Amazon EC2

Architecture Overview

EC2 Instance
⬇
Attached EBS Volume (Block Storage)
⬇
Mounted EFS (File Storage)
⬇
S3 Bucket (Object Storage for static/backup data)

# Object Storage – Amazon S3
Tasks Performed:
Created an S3 bucket
Uploaded files
Downloaded files
Configured bucket permissions

# Commands Used (AWS CLI Example)
```
aws s3 mb s3://my-storage-bucket
aws s3 cp file.txt s3://my-storage-bucket/
aws s3 ls s3://my-storage-bucket/
```

# Block Storage – Amazon EBS
Tasks Performed:
Created EBS volume
Attached volume to EC2
Formatted the disk
Mounted volume to directory

Linux Commands Used
```
lsblk
sudo mkfs.ext4 /dev/xvdf
sudo mount /dev/xvdf /data
```

# File Storage – Amazon EFS
Tasks Performed:
Created EFS file system
Mounted to EC2 instance
Shared files across instances

