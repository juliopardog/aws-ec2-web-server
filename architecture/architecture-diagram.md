# AWS EC2 Web Server Architecture

```mermaid
graph TD
    U[User Browser] --> EC2[Amazon EC2 Web Server]
    EC2 -. protected by .-> SG[Security Group]
    EC2 -. monitored by .-> CW[CloudWatch]
    EC2 --> VPC[VPC Network]
```
