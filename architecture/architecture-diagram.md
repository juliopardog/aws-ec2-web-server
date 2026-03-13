# AWS EC2 Web Server Architecture

```mermaid
graph TD
    U[User Browser] --> EC2[EC2 Web Server]

    subgraph VPC[VPC Network]
        EC2 --> SG[Security Group]
    end

    EC2 --> CW[CloudWatch Monitoring]
```
