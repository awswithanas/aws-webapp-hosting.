# AWS Web Application Hosting Project

## Overview
This project demonstrates hosting a highly available and scalable web application on AWS using core services like EC2, RDS, S3, and ALB. The goal is to build an architecture similar to real-world production systems.

## Architecture
- **VPC** with public and private subnets across 2 Availability Zones.
- **Application Load Balancer (ALB)** to distribute traffic across EC2 instances.
- **Auto Scaling Group (ASG)** for dynamic scaling of EC2.
- **RDS (Multi-AZ)** for high availability database.
- **S3** bucket for storing static assets (HTML, images).
- **CloudWatch** for monitoring and alerts.
- **IAM** for secure access and role-based permissions.


## Steps Implemented
1. Created a VPC with public and private subnets.
2. Launched EC2 instances in private subnets and attached them to an Auto Scaling Group.
3. Configured Application Load Balancer in public subnets.
4. Set up RDS in Multi-AZ mode with automated backups.
5. Used S3 for storing and serving static content.
6. Enabled CloudWatch alarms for instance health and CPU usage.
7. Configured Route 53 domain to point to the ALB.

## Key Learnings
- Importance of Multi-AZ for high availability.
- How Auto Scaling helps handle sudden traffic spikes.
- Benefits of separating public and private subnets.
- Using CloudWatch to monitor and troubleshoot performance.

## Future Enhancements
- Add WAF for web application security.
- Use CloudFront for global content delivery.
- Automate infrastructure using CloudFormation/Terraform.
