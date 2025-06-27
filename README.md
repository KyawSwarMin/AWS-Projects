# AWS Architecture Lab

This project demonstrates a scalable and secure AWS architecture designed for a web application. The architecture incorporates various AWS services to ensure high availability, fault tolerance, and security.

## Architecture Overview

![AWS Architecture Diagram](https://miro.medium.com/max/1400/1*3v8k5K1_7Y9Q5Q5Q5Q5Q5Q.png)

The architecture consists of the following components:

### Frontend Layer
- **S3**: Static website hosting for frontend assets

### Application Layer
- **EC2 Auto Scaling Group**: For horizontal scaling of application servers
- **Elastic Load Balancer (ALB)**: Distributes traffic across instances

### Data Layer
- **RDS (PostgreSQL)**: Managed relational database with Multi-AZ deployment
- 
### Security
- **Security Groups & NACLs**: Network-level security
- **IAM**: Fine-grained access control

### Monitoring & Operations
- **CloudWatch**: Monitoring and logging
- **SNS**: Alert notifications

## Deployment Steps

1. **Set up VPC with public and private subnets**
2. **Configure security groups and NACLs**
3. **Deploy RDS database in private subnets**
4. **Create EC2 launch template and Auto Scaling Group**
5. **Set up Application Load Balancer**
6. **Configure CloudFront with S3 origin**
7. **Implement monitoring and alerts**

## Best Practices Implemented

- Multi-AZ deployment for high availability
- Infrastructure as Code (IaC) using Terraform
- Encryption at rest and in transit
- Regular automated backups
- Horizontal scaling for variable loads

## Prerequisites

- AWS account with appropriate permissions
- Terraform installed (for infrastructure provisioning)
- Basic understanding of AWS services

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
