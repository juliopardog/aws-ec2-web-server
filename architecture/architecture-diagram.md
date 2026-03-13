# AWS EC2 Web Server Architecture

```mermaid
graph TD
    User[User Browser] --> ALB[Application Load Balancer]
    ALB --> EC2[EC2 Web Server]
    EC2 --> CW[CloudWatch Monitoring]
    EC2 --> SG[Security Group]
    SG --> VPC[VPC Network]
