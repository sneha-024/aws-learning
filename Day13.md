# AWS Day 13 — Amazon S3 and Static Website Hosting

# What I Learned Today

Today I learned about Amazon S3, object storage, storage classes, bucket permissions, and static website hosting.

I also hosted my first static website using an S3 bucket.

---

# What is Amazon S3?

Amazon Simple Storage Service (S3) is an object storage service used to store and retrieve data from the cloud.

S3 is highly durable, scalable, and widely used across AWS services.

Common Use Cases:

* File storage
* Backup and recovery
* Static website hosting
* Log storage
* Media storage

---

# S3 Terminology

## Bucket

A bucket is a container used to store objects.

Example:

```text
my-static-website-bucket
```

Bucket names must be globally unique.

---

## Object

An object is a file stored inside a bucket.

Examples:

* index.html
* image.png
* notes.pdf

Every object consists of:

* Data
* Metadata
* Unique key

---

# Storage Classes

AWS provides multiple storage classes for different use cases.

| Storage Class           | Use Case                    |
| ----------------------- | --------------------------- |
| S3 Standard             | Frequently accessed data    |
| S3 Intelligent-Tiering  | Automatic cost optimization |
| S3 Standard-IA          | Infrequent access           |
| S3 Glacier              | Archival storage            |
| S3 Glacier Deep Archive | Long-term archive           |

---

# Permissions

S3 permissions determine who can access bucket contents.

Methods:

* IAM Policies
* Bucket Policies
* ACLs (Access Control Lists)

Best Practice:

Avoid making buckets public unless required.

---

# Static Website Hosting

S3 can host static websites containing:

* HTML
* CSS
* JavaScript

Static websites do not require a web server such as nginx.

---

# Practical Tasks Performed

* Created an S3 bucket
* Uploaded website files
* Configured bucket permissions
* Enabled static website hosting
* Accessed website using the public URL

---

# Static Website URL

Replace this with your actual URL after deployment:

```text
https://your-bucket-name.s3-website-region.amazonaws.com
```

---

# Key Takeaways

* S3 is an object storage service.
* Buckets store objects.
* Storage classes help optimize cost.
* Bucket permissions control access.
* S3 can host static websites without managing servers.
* Static website hosting is one of the simplest deployment methods in AWS.

---

# Milestone

Successfully deployed my first website using Amazon S3.
