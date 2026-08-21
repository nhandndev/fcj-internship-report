---
title: "AWS IAM Access Control"
weight: 5
chapter: false
pre: " <b> 1.1.5 </b> "
---

### Overview

AWS Identity and Access Management (IAM) is the access control service used to manage identities and permissions in AWS. In this lab, I practiced creating IAM users, groups, roles, and switching roles to understand secure access management.

### Lab Contents

1. Introduction to IAM.
2. Create IAM Group and IAM User.
3. Create IAM Role and IAM User.
4. Switch Role.
5. Clean up resources.

### Security Objectives

* Manage users through groups instead of assigning permissions one by one.
* Apply IAM policies to control allowed actions.
* Use IAM roles for temporary access.
* Practice the principle of least privilege.

### What I Completed

* Created an IAM Group for organizing users.
* Created an IAM User and assigned access through the group.
* Created an IAM Role for controlled access.
* Practiced Switch Role from the AWS Management Console.
* Cleaned up lab resources after completing the practice.

### Lab Notes

I started by reviewing the IAM introduction to understand the difference between users, groups, policies, and roles. After that, I followed the lab flow step by step in the AWS Console.

The user and group part helped me understand how permissions can be managed more cleanly. Instead of attaching permissions directly to each user, I can put users into a group and manage permissions from that group.

The role section was the most useful part of the lab. I learned that a role is not a normal login user. It is used when temporary permissions are needed, and the Switch Role feature makes it possible to change permission context without sharing long-term credentials.

### References Checked

* AWS Study Group IAM Access Control lab.
* AWS IAM documentation about policies and roles.
* AWS Management Console during hands-on practice.

### Summary of Today's Learning

1. **IAM Group and User**: Groups make permission management easier and more consistent.
2. **IAM Role**: Roles are useful for temporary and controlled access.
3. **Least privilege**: Permissions should be limited to only what is required for the task.
