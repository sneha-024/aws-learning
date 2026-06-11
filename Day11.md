# AWS Day 11 — Amazon EC2

# What I Learned Today

Today I launched my first AWS EC2 instance and connected to it using SSH.

This was my first experience working with a cloud server instead of a local machine.

---

# What is EC2?

Amazon Elastic Compute Cloud (EC2) is a service that provides virtual servers in the cloud.

EC2 allows users to launch, configure, and manage servers on demand.

Common Use Cases:

* Web hosting
* Application hosting
* Development environments
* Testing environments

---

# Important EC2 Concepts

## AMI (Amazon Machine Image)

An AMI is a template used to launch EC2 instances.

Examples:

* Ubuntu
* Amazon Linux
* Red Hat Enterprise Linux

---

## Instance Type

Defines CPU, memory, and networking capacity.

Example:

```text
t2.micro
```

Used under the AWS Free Tier.

---

## Key Pair

Used for secure SSH access to Linux instances.

Components:

* Public Key
* Private Key (.pem file)

The private key must be stored securely.

---

## Security Group

Acts as a virtual firewall.

Controls:

* Inbound Traffic
* Outbound Traffic

Example Rules:

* SSH (22)
* HTTP (80)

---

# Practical Tasks Performed

* Created an EC2 instance
* Selected Ubuntu AMI
* Created a key pair
* Configured security groups
* Connected using SSH
* Installed nginx
* Verified nginx service status
* Accessed the web server using the public IP address

---

# Commands Used

```bash
sudo apt update
sudo apt install nginx -y
sudo systemctl status nginx
```

---

# Key Takeaways

* EC2 provides virtual servers in the cloud.
* AMIs act as server templates.
* Security groups control network access.
* Key pairs are required for secure SSH authentication.
* Public IP addresses allow remote access.
* nginx can be deployed on EC2 to host web content.

---

# Milestone

Successfully launched and managed my first cloud server on AWS.

