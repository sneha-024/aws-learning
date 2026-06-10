# AWS Day 10 — Cloud Computing Fundamentals and IAM

# What I Learned Today

Today I learned the fundamentals of cloud computing, AWS global infrastructure, and Identity and Access Management (IAM).

Understanding IAM is critical because it controls who can access AWS resources and what actions they can perform.

---

# What is Cloud Computing?

Cloud computing is the delivery of computing resources over the internet instead of managing physical infrastructure.

Examples of resources:

* Virtual Servers
* Storage
* Databases
* Networking
* Security Services

Benefits:

* Pay as you go
* Scalability
* High availability
* Reduced infrastructure management

---

# On-Premises vs Cloud

| On-Premises                | Cloud                     |
| -------------------------- | ------------------------- |
| Own hardware               | Provider manages hardware |
| High upfront cost          | Pay only for usage        |
| Manual scaling             | Easy scaling              |
| Maintenance responsibility | Managed by cloud provider |

---

# What is AWS?

Amazon Web Services (AWS) is a cloud computing platform that provides a wide range of services including compute, storage, networking, security, databases, and analytics.

AWS follows a global infrastructure model.

---

# AWS Global Infrastructure

## Region

A Region is a physical geographic location where AWS operates data centers.

Examples:

* ap-south-1 (Mumbai)
* us-east-1 (N. Virginia)
* eu-west-1 (Ireland)

---

## Availability Zone (AZ)

An Availability Zone is one or more isolated data centers within a region.

Example:

```text
Mumbai Region
├── ap-south-1a
├── ap-south-1b
└── ap-south-1c
```

Benefits:

* High availability
* Fault tolerance

---

## Edge Locations

Edge locations are used by AWS services such as CloudFront to deliver content closer to users.

Benefits:

* Lower latency
* Faster content delivery

---

# Identity and Access Management (IAM)

IAM is the AWS service used to manage authentication and authorization.

Questions IAM answers:

* Who can access AWS?
* What can they access?
* What actions can they perform?

---

# IAM Components

## IAM User

Represents an individual person or application.

Example:

```text
Sneha
Developer
Administrator
```

---

## IAM Group

Collection of IAM users.

Example:

```text
Developers Group
Admins Group
```

Permissions can be assigned to groups instead of individual users.

---

## IAM Policy

A JSON document that defines permissions.

Example:

```text
Allow EC2 Read Access
Allow S3 Full Access
```

Policies determine what actions are allowed or denied.

---

## IAM Role

A role provides temporary permissions.

Common use cases:

* EC2 accessing S3
* Lambda accessing DynamoDB
* Cross-account access

Unlike users, roles do not have permanent credentials.

---

# AWS Account Security Best Practices

## Root User

The root account has full control over the AWS account.

Best Practice:

* Do not use the root account for daily tasks.
* Use IAM users instead.

---

## Multi-Factor Authentication (MFA)

MFA adds an additional security layer.

Authentication requires:

* Password
* Verification code

Benefits:

* Improved account security
* Protection against credential theft

---

# Practical Tasks Performed

* Explored AWS global infrastructure
* Understood regions and availability zones
* Learned IAM concepts
* Reviewed users, groups, roles, and policies
* Enabled security best practices awareness
* Understood the importance of MFA

---

# Key Takeaways

* Cloud computing eliminates the need to manage physical infrastructure.
* AWS provides scalable and globally distributed services.
* Regions contain multiple Availability Zones.
* IAM controls authentication and authorization.
* Policies define permissions.
* Roles provide temporary access.
* Root account usage should be minimized.
* MFA is a critical security control.

---
