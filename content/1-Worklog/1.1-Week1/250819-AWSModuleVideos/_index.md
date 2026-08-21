---
title: "AWS Module Video Notes"
weight: 3
chapter: false
pre: " <b> 1.1.3 </b> "
---

### Overview

This note summarizes the preparation work from watching AWS learning videos and reviewing the Explore AWS Services module before starting the hands-on labs.

### Topics Reviewed

* AWS global infrastructure and basic cloud concepts.
* The purpose of AWS core services such as IAM, VPC, EC2, Budgets, and Support.
* FCJ learning path and expected Week 1 lab outcomes.
* Basic security mindset when using a cloud account.

### Study Notes

I used this day mainly for watching overview videos and reading the module pages before touching the AWS Console. The goal was not to finish a lab yet, but to understand what each service is used for.

The most important point I noted is that AWS services are usually connected. IAM controls access, Budgets helps control spending, VPC provides the network layer, and EC2 runs compute resources inside that network. Because of that, I should understand the basic purpose of each service before doing the hands-on steps.

### Questions Prepared

* What should be done with the root user after creating an AWS account?
* When should an IAM user be used instead of the root user?
* Why should a budget alert be created before doing labs?
* What is the difference between a public subnet and a private subnet?

### Key Takeaways

* IAM is used to control who can access AWS resources and what actions they can perform.
* VPC provides the networking foundation for running cloud workloads.
* AWS Budgets helps monitor spending and avoid unexpected costs.
* AWS Support is used when users need help with account, billing, or technical issues.

### References Checked

* AWS Study Group Cloud Journey module pages.
* AWS official documentation for IAM, VPC, and AWS Budgets.
* YouTube overview videos about AWS basic services.

### Summary of Today's Learning

1. **Module preparation**: Built a clearer picture of the services before doing hands-on labs.
2. **Service relationships**: Understood that IAM, VPC, and EC2 are connected in many AWS architectures.
3. **Cloud responsibility**: Learned that security and cost control should be considered from the beginning.
