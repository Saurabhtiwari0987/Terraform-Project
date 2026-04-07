# Terraform AWS Projects Collection

This repository contains multiple Terraform projects covering AWS infrastructure provisioning, modularization, backend configuration, and real-world DevOps scenarios.

Each folder represents a separate Terraform project with specific use‑cases.

---

# 📁 Project Structure

## 1. aws-IAM-management

### Description

This project is used to manage AWS IAM resources using Terraform.

### Resources Created

* IAM Users
* IAM Groups
* IAM Roles
* IAM Policies
* User Login Profiles

### Use Case

* User access management
* Role based access control
* DevOps team permission setup

### Commands

```bash
terraform init
terraform plan
terraform apply
```

---

## 2. aws-ec2

### Description

This project provisions EC2 instances using Terraform.

### Resources Created

* EC2 Instance
* Security Group
* Key Pair

### Use Case

* Application hosting
* Testing infrastructure

---

## 3. aws-s3

### Description

This project creates AWS S3 buckets.

### Resources Created

* S3 Bucket
* Versioning
* Bucket Policy

### Use Case

* Static website hosting
* Storage
* Backup

---

## 4. aws-vpc-ec2-nginx

### Description

This project creates a custom VPC, EC2 instance, and installs NGINX.

### Resources Created

* VPC
* Subnet
* Internet Gateway
* Route Table
* EC2 Instance
* Security Group
* NGINX Installation

### Use Case

* Web server deployment
* Custom networking

---

## 5. aws-vpc

### Description

This project creates AWS VPC infrastructure.

### Resources Created

* VPC
* Subnet
* Internet Gateway
* Route Table

### Use Case

* Network isolation
* Infrastructure foundation

---

## 6. proj-static-website

### Description

This project deploys static website using S3.

### Resources Created

* S3 Bucket
* Static Website Hosting
* Bucket Policy

### Use Case

* Portfolio website
* Static application hosting

---

## 7. testing-local-module

### Description

This project demonstrates local Terraform modules.

### Features

* Module reuse
* Local module testing

### Use Case

* Terraform modularization

---

## 8. tf-backend

### Description

This project configures Terraform remote backend.

### Resources Created

* S3 Bucket
* DynamoDB Table

### Use Case

* Remote state storage
* State locking

---

## 9. tf-cli-workspace

### Description

This project demonstrates Terraform CLI workspaces.

### Features

* Multiple environments
* Dev / Stage / Prod

### Commands

```bash
terraform workspace new dev
terraform workspace new prod
terraform workspace list
```

---

## 10. tf-data-sources

### Description

This project demonstrates Terraform data sources.

### Examples

* Existing VPC
* Existing AMI
* Existing Security Group

### Use Case

* Using existing infrastructure

---

## 11. tf-functions

### Description

This project demonstrates Terraform functions.

### Functions Used

* lookup
* join
* element
* length
* file

### Use Case

* Dynamic configuration

---

## 12. tf-module-vpc

### Description

This project demonstrates reusable VPC module.

### Features

* Reusable modules
* Parameterized variables

---

## 13. tf-multi-resources

### Description

This project creates multiple AWS resources.

### Resources

* Multiple EC2 Instances
* Multiple S3 Buckets

### Use Case

* Bulk resource creation

---

## 14. tf-operators-exps

### Description

This project demonstrates Terraform operators.

### Operators

* Conditional operators
* Arithmetic operators
* Logical operators

---

## 15. tf-own-module-VPC

### Description

This project creates custom VPC module.

### Features

* Custom module
* Reusable infrastructure

---

# 🚀 How to Use

Clone Repository

```bash
git clone <repo-url>
cd terraform-projects
```

Initialize Terraform

```bash
terraform init
```

Plan Infrastructure

```bash
terraform plan
```

Apply Infrastructure

```bash
terraform apply
```

Destroy Infrastructure

```bash
terraform destroy
```

---

# 📌 Requirements

* Terraform
* AWS CLI
* AWS Account
* IAM User with Access Keys

---

# 🔧 Configure AWS CLI

```bash
aws configure
```

Enter:

* Access Key
* Secret Key
* Region

---

# 👨‍💻 Author

DevOps Terraform Practice Repository

---

# 📚 Learning Topics Covered

* Terraform Basics
* AWS Infrastructure
* Modules
* Backend
* Workspaces
* Functions
* Data Sources
* VPC
* EC2
* S3
* IAM

---

# ⭐ Purpose

This repository is created for:

* DevOps Practice
* Terraform Learning
* AWS Automation
* Interview Preparation

---



---

# 📢 Notes

Each folder is independent project. Navigate to folder before running Terraform commands.

Example:

```bash
cd aws-ec2
terraform init
terraform apply
```

---

# ✅ Best Practices

* Use remote backend
* Use modules
* Use variables
* Use outputs

---

# 🏁 End

Happy Learning Terraform 🚀
