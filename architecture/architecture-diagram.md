# AWS EC2 Web Server Architecture

```mermaid
graph TD
    User[User Browser] --> ALB[Application Load Balancer]

    ALB --> EC1[EC2 Web Server 1]
    ALB --> EC2[EC2 Web Server 2]

    EC1 --> SG[Security Group]
    EC2 --> SG

    SG --> VPC[VPC Network]

    CW[CloudWatch Monitoring] --> EC1
    CW --> EC2
```
