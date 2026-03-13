# Deployment Guide

## Overview
This project deploys a simple web server using AWS EC2 and an automated user-data script.

## Requirements
- AWS account
- Access to EC2 service

## Deployment Steps

1. Open the AWS Management Console
2. Navigate to EC2
3. Click "Launch Instance"
4. Select Amazon Linux 2
5. Choose instance type t2.micro
6. Configure security group to allow HTTP (port 80)
7. Paste the user-data script from scripts/user-data.sh into the User Data section
8. Launch the instance

## Verification

After the instance launches:

1. Copy the public IPv4 address
2. Open the address in a web browser
3. You should see the message:

AWS EC2 Web Server Deployed by Julio

## Architecture Components

- EC2 instance running Apache
- Security Group allowing HTTP traffic
- CloudWatch monitoring

## Author
Julio Pardo
