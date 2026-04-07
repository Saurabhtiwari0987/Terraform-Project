# 🚀 Terraform Complete Learning Repository

This repository contains **complete Terraform learning projects** from **beginner to advanced level** including AWS infrastructure provisioning, modules, backend, workspaces, variables, functions and real-world DevOps scenarios.

This documentation explains **complete Terraform concepts** so anyone reading this repository can understand the **entire Terraform workflow**.

---

# 📌 What is Terraform?

Terraform is an **Infrastructure as Code (IaC)** tool developed by HashiCorp that allows you to **create, manage, and provision infrastructure using code**.

Instead of creating resources manually in AWS Console, Terraform allows you to define infrastructure in `.tf` files.

Example:

* EC2 Instance
* VPC
* S3 Bucket
* IAM Users
* Load Balancer

All can be created using Terraform.

---

# 🎯 Why Use Terraform?

## Problems Without Terraform

* Manual infrastructure creation
* No version control
* No automation
* Difficult to manage multiple environments
* Human errors

## Benefits of Terraform

* Infrastructure as Code
* Automation
* Version control
* Reusability
* Multi‑cloud support
* Team collaboration

---

# ⚙️ Terraform Workflow

Terraform follows a standard workflow:

## Step 1 — Write Code

Create `.tf` files

Example:

```
main.tf
variables.tf
provider.tf
outputs.tf
```

---

## Step 2 — Initialize Terraform

```
terraform init
```

This downloads:

* Provider plugins
* Modules
* Backend configuration

---

## Step 3 — Terraform Plan

```
terraform plan
```

This command shows:

* What Terraform will create
* What Terraform will update
* What Terraform will destroy

---

## Step 4 — Terraform Apply

```
terraform apply
```

This command creates infrastructure.

---

## Step 5 — Terraform Destroy

```
terraform destroy
```

Deletes infrastructure.

---

# 📁 Terraform Directory Structure

Typical Terraform Project Structure:

```
terraform-project
│
├── main.tf
├── variables.tf
├── provider.tf
├── outputs.tf
├── terraform.tfvars
└── backend.tf
```

---

# 📄 main.tf

Main Terraform file.

Contains:

* Resources
* Modules
* Data sources

Example:

```
resource "aws_instance" "example" {
  ami = "ami-id"
  instance_type = "t2.micro"
}
```

---

# 📄 provider.tf

Defines cloud provider.

Example:

```
provider "aws" {
  region = "us-east-1"
}
```

---

# 📄 variables.tf

Defines variables.

Example:

```
variable "instance_type" {
 default = "t2.micro"
}
```

---

# 📄 terraform.tfvars

Used to assign values.

Example:

```
instance_type = "t2.micro"
```

---

# 📄 outputs.tf

Used to print output.

Example:

```
output "instance_ip" {
 value = aws_instance.example.public_ip
}
```

---

# 📌 What is Terraform State?

Terraform State file stores:

* Infrastructure information
* Resource IDs
* Configuration details

File name:

```
terraform.tfstate
```

---

# Why Terraform State is Important?

Terraform compares:

* Current Infrastructure
* Desired Infrastructure

Then decides:

* Create
* Update
* Delete

---

# 📌 What is Remote Backend?

Remote backend stores state file remotely.

Example:

* AWS S3
* Terraform Cloud

Benefits:

* Team collaboration
* State locking
* Secure storage

---

# 📌 What is State Locking?

Prevents multiple users from modifying infrastructure simultaneously.

Terraform uses:

* DynamoDB

Example:

```
S3 + DynamoDB
```

---

# 📌 What is Terraform Variables?

Variables make code reusable.

Example:

```
variable "region" {}
```

Use:

```
var.region
```

---

# 📌 Terraform Workspaces

Used for multiple environments.

Example:

* dev
* stage
* prod

Commands:

```
terraform workspace new dev
terraform workspace select dev
```

---

# 📌 Terraform Modules

Modules allow reusable infrastructure.

Example:

```
module "vpc" {
 source = "./vpc"
}
```

---

# 📌 Terraform Data Sources

Used to fetch existing infrastructure.

Example:

```
data "aws_ami" "example" {}
```

---

# 📌 Terraform Functions

Used for dynamic values.

Examples:

* lookup
* join
* length
* element

---

# 📁 Repository Projects Explanation

## aws-IAM-management

Manage IAM users, roles and policies.

Learning:

* IAM management
* Access control

---

## aws-ec2

Creates EC2 instance.

Learning:

* EC2 provisioning

---

## aws-s3

Creates S3 bucket.

Learning:

* Storage provisioning

---

## aws-vpc

Creates VPC networking.

Learning:

* Networking

---

## aws-vpc-ec2-nginx

Creates:

* VPC
* EC2
* Nginx

Learning:

* Full stack infra

---

## proj-static-website

Deploy static website.

---

## testing-local-module

Testing modules.

---

## tf-backend

Remote backend setup.

---

## tf-cli-workspace

Workspace example.

---

## tf-data-sources

Data source example.

---

## tf-functions

Functions example.

---

## tf-module-vpc

Reusable VPC module.

---

## tf-multi-resources

Multiple resource creation.

---

## tf-operators-exps

Operators example.

---

## tf-own-module-VPC

Custom VPC module.

---

# 📚 Learning Outcome

After completing this repository:

You will learn:

* Terraform Basics
* AWS Infrastructure
* Modules
* Workspaces
* Backend
* State file
* Variables
* Functions
* Data Sources

---

# 🎯 Goal

This repository helps:

* DevOps Engineers
* Cloud Engineers
* Beginners
* Interview Preparation

---

# 🚀 Happy Learning Terraform
