# Terraform

Terraform is an Infrastructure as Code (IaC) tool by HashiCorp that lets you define, provision, and manage infrastructure using configuration files.

## Key Concepts:
1. Provider
A provider is a plugin that allows Terraform to interact with cloud platforms or services (AWS, Azure, GCP, etc.).

```
provider "aws" {
  region = "us-east-1"
}
```

2. Resource
Resources define the infrastructure components you want to create.
```
resource "aws_instance" "example" {
  ami           = "ami-0abcd1234"
  instance_type = "t2.micro"
}
```

3. Variables
Variables make configurations reusable and flexible.
```
variable "instance_type" {
  default = "t2.micro"
}
```

4. Outputs
Outputs display useful values after infrastructure is created.
```
output "instance_id" {
  value = aws_instance.example.id
}
```

5. State
Terraform uses a state file to track real infrastructure vs configuration.
- Stored locally by default (terraform.tfstate)
- Can be stored remotely (S3, Terraform Cloud)

## Common Terraform Commands
```
terraform init      # Initialize project
terraform plan      # Preview changes
terraform apply     # Create/update infrastructure
terraform destroy   # Delete infrastructure
```