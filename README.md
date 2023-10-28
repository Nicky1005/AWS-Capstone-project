# AWS-Capstone-project
# Employee Profile Management System for XYZ Company

## Project Overview
The Employee Profile Management System for XYZ Company is designed to allow new employees to input their information and upload photos, while existing employees can access their information. This system is built using various AWS services configured within a Virtual Private Cloud (VPC).

## System Components
1. **VPC Setup**:
   - Configured with a Load Balancer, Application EC2 instance, and RDS Database.
   - Comprising one public and two private subnets for better security and isolation.

2. **Load Balancer and Auto Scaling Group**:
   - Utilizes an Auto Scaling Group to dynamically adjust the number of EC2 instances.
   - Load balancer distributes incoming application traffic across multiple instances.

3. **Database Services**:
   - RDS DB Instance: Hosts the main relational database for employee information.
   - DynamoDB Table: For managing specific types of data and configurations.

4. **S3 Bucket**:
   - Utilized for storing and managing uploaded photos and other related data.

5. **Domain Name Mapping**:
   - Obtained domain name and mapped it with the Load Balancer for easy access.

6. **Instance Profile and Permissions**:
   - Configured an instance profile with permissions to access RDS, DynamoDB, and the S3 bucket.
   - The profile is attached to the EC2 instances being launched for seamless access to required services.

## Deployment and Usage
### Steps for Deployment:
1. Set up the VPC with appropriate subnets and instances.
2. Create and configure the Load Balancer and Auto Scaling Group.
3. Establish the RDS Database and DynamoDB Table.
4. Create and configure the S3 bucket for file storage.
5. Map the domain name to the Load Balancer.
6. Attach the instance profile to EC2 instances being launched.

### Usage:
- New employees can input their information and upload photos via the provided application interface.
- Existing employees can access their information through the system.

