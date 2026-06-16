# AWS Day 12 — VPC, Subnets and Security Groups

# What I Learned Today

Today I learned the networking foundation of AWS, including Virtual Private Clouds (VPCs), Subnets, and Security Groups.

Since I already have networking experience, these concepts were easier to relate to traditional on-premises networking.

---

# What is a VPC?

A Virtual Private Cloud (VPC) is a logically isolated network inside AWS.

It allows users to create and manage their own cloud network.

A VPC contains:

* Subnets
* Route Tables
* Internet Gateways
* Security Groups
* Network ACLs

Think of a VPC as a private data center network running inside AWS.

---

# What is a Subnet?

A subnet is a smaller network segment inside a VPC.

Subnets help organize resources and control traffic flow.

Types:

## Public Subnet

Resources can communicate with the internet through an Internet Gateway.

Examples:

* Web Servers
* Load Balancers

---

## Private Subnet

Resources do not have direct internet access.

Examples:

* Databases
* Internal Application Servers

---

# What is a Security Group?

A Security Group acts as a virtual firewall for AWS resources.

Security Groups control:

* Inbound Traffic
* Outbound Traffic

Example:

Allow:

* SSH (22)
* HTTP (80)
* HTTPS (443)

Block everything else.

---

# Why Security Groups are Important

Security Groups help protect cloud resources by limiting who can access them.

Example:

```text
Allow SSH only from my IP address.
Allow HTTP from anywhere.
```

---

# Security Groups vs Traditional Firewalls

| Security Group            | Traditional Firewall          |
| ------------------------- | ----------------------------- |
| Cloud-based               | Physical or software firewall |
| Attached to AWS resources | Attached to network devices   |
| Stateful                  | Can be stateful or stateless  |
| Controls instance traffic | Controls network traffic      |

---

# VPC vs Traditional Network

| AWS Concept      | Traditional Networking Equivalent |
| ---------------- | --------------------------------- |
| VPC              | Enterprise Network                |
| Subnet           | VLAN / Network Segment            |
| Security Group   | Stateful Firewall Rule Set        |
| Internet Gateway | Edge Router / Internet Connection |
| Route Table      | Routing Table                     |
| EC2 Instance     | Physical or Virtual Server        |

---

# Traditional Network Example

```text
Office Network
├── User VLAN
├── Server VLAN
├── Firewall
└── Internet Router
```

---

# AWS Equivalent

```text
AWS VPC
├── Public Subnet
├── Private Subnet
├── Security Groups
└── Internet Gateway
```

---

# Practical Tasks Performed

* Explored the default VPC
* Reviewed subnet configuration
* Examined route tables
* Studied security group rules
* Compared AWS networking with traditional networking concepts

---

# Key Takeaways

* A VPC is a private network inside AWS.
* Subnets divide a VPC into smaller network segments.
* Security Groups act as stateful firewalls.
* AWS networking closely resembles traditional networking concepts.
* Existing networking knowledge can be directly applied to cloud networking.

---

# Personal Observation

Coming from a networking background, AWS networking concepts felt familiar because many cloud networking components are virtualized versions of traditional networking concepts such as VLANs, routing, segmentation, and firewall rules.
