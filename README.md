# Infrastructure-as-Code
Automate cloud infra with Terraform. Define stack as code for easy versioning, maintenance &amp; reproducibility. Reliable IaC for cloud management.

Welcome to the Infrastructure-as-Code (IaC) repository! This project aims to automate the provisioning and management of cloud infrastructure using Terraform, a popular open-source IaC tool. With IaC, we can define our entire infrastructure stack as code, making it easier to version, maintain, and reproduce our infrastructure consistently and reliably.

<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code/blob/main/Infrastructure-As-Code.jpg" width="800" height="450" alt="Example Image">


### Terraform Documantation for AWS 
https://registry.terraform.io/providers/hashicorp/aws/latest/docs
 
### Connect AWS to Terraform 

```tf
provider "aws" {
  region     = "us-west-2"
  access_key = "my-access-key"
  secret_key = "my-secret-key"
}
```

## Terraform Workflow
<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Terraform%20Workflow.png" alt="Example Image">
