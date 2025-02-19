# Basic Terraform Syntax

Terraform uses **HashiCorp Configuration Language (HCL)** to define infrastructure resources in a declarative way. Below are some key syntax elements:

## 1. Declaring a Provider
```hcl
provider "aws" {
  region = "us-east-1"
}
```
This tells Terraform to use AWS as the cloud provider and sets the region.

## 2. Defining Resources
```hcl
resource "aws_instance" "example" {
  ami           = "ami-12345678"
  instance_type = "t2.micro"
}
```
This creates an AWS EC2 instance with a specific AMI and instance type.

## 3. Using Variables
```hcl
variable "instance_type" {
  default = "t2.micro"
}

resource "aws_instance" "example" {
  ami           = "ami-12345678"
  instance_type = var.instance_type
}
```
Variables make the configuration more flexible.

## 4. Outputs
```hcl
output "instance_ip" {
  value = aws_instance.example.public_ip
}
```
Outputs help retrieve information about created resources.

## 5. Terraform Commands
- **`terraform init`** – Initializes Terraform in the working directory.
- **`terraform plan`** – Shows what Terraform will create/update.
- **`terraform apply`** – Applies the configuration and creates resources.
- **`terraform destroy`** – Deletes all managed resources.
