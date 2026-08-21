---
title: "Amazon VPC Learning Notes"
weight: 6
chapter: false
pre: " <b> 1.1.6 </b> "
---

### Overview

Amazon Virtual Private Cloud (Amazon VPC) is used to create an isolated network environment in AWS. Today, I focused on learning the VPC workflow and understanding the role of each networking component before doing a full deployment.

### Topics Studied

* VPC and CIDR block planning.
* Public and private subnets.
* Route tables and routing rules.
* Internet Gateway for public internet access.
* Security Groups as instance-level firewall rules.
* Basic relationship between VPC networking and EC2 deployment.

### Practice Plan

* Create a VPC with an appropriate CIDR block.
* Create subnets for different availability zones.
* Attach an Internet Gateway.
* Configure route tables for public subnet access.
* Review Security Group rules before launching EC2 resources.

### Summary of Today's Learning

1. **VPC foundation**: VPC is the base network layer for many AWS workloads.
2. **Subnet design**: Public and private subnets separate resources by access level.
3. **Routing flow**: Internet access requires a correct route table and Internet Gateway configuration.
