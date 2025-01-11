## Deployment of ALB with an ASG using Terraform

This project explains the automated deployment process of an Application Load Balancer (ALB) with an Auto-scaling Group (ASG) using `Terrform`:
- AWS Autoscaling group spanning three subnets.
- IAM role attached to Autoscaling instances to access other AWS services
- Application Load Balancer attached to the Autoscaling group

## Prerequisites

- The latest Terraform binary is installed and configured in your system.
- `AWS CLI` is installed and configured with a valid AWS account with permission to deploy the autoscaling group and application load balancer.
- If you are using an ec2 instance to run Terraform, ensure you attach an IAM role with permission to create ASG and ALB.

## Setup Architecture & Overview

![High-Level Architecture](./images/lb-asg-workflow.gif)