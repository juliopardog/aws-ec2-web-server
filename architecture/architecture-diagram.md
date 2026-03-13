# AWS EC2 Web Server Architecture

```mermaid
graph TD
    U[User Browser] --> EC2[Amazon EC2 Web Server]

    EC2 -. protected by .-> SG[Security Group]
    EC2 -. monitored by .-> CW[CloudWatch]

    subgraph VPC[VPC Network]
        EC2
        SG
    end
```

## Architecture Overview

This project deploys an Apache web server on an Amazon EC2 instance inside a VPC.  
A security group controls inbound HTTP traffic, and Amazon CloudWatch collects monitoring metrics for the instance.
