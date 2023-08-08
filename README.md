# Infrastructure-as-Code
Automate cloud infra with Terraform. Define stack as code for easy versioning, maintenance &amp; reproducibility. Reliable IaC for cloud management.

Welcome to the Infrastructure-as-Code (IaC) repository! This project aims to automate the provisioning and management of cloud infrastructure using Terraform, a popular open-source IaC tool. With IaC, we can define our entire infrastructure stack as code, making it easier to version, maintain, and reproduce our infrastructure consistently and reliably.

<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code/blob/main/Infrastructure-As-Code.jpg" width="800" height="400" alt="Example Image">


### Terraform Documantation for AWS 
https://registry.terraform.io/providers/hashicorp/aws/latest/docs

## Terraform Installation
<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Terraform%20Installation.png" width="800" height="400" alt="Example Image">

 
### Connect AWS to Terraform 

```tf
provider "aws" {
  region     = "us-west-2"
  access_key = "my-access-key"
  secret_key = "my-secret-key"
}
```

Provider

Is like a Platform Cloud Provider e.g. AWS, GCP, Azure

## Terraform Workflow

<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Terraform%20Workflow%2002.png" width="800" height="300" alt="Terraform Workflow Basics">

<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Terraform%20Workflow.png" width="800" height="400" alt="Terraform Workflow">

## Terraform Language Basics
* Code in the Terraform language is stored in plain text files with the ```.tf``` file extension. 
* There is also a JSON-based variant of the language that is named with the ```.tf.json``` file extension.
* We can call the files containing terraform code as Terraform Configuration Files or Terraform Manifests

<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Terraform%20Language%20Basics%20%E2%80%93%20Configuration%20Syntax.png" width="800" height="300" alt="Terraform Language Basics – Configuration Syntax">

## Terraform code to Connect with EC2 Instance

```tf
provider "aws" {
  region = "us-west-2"  # Set your desired AWS region here
}

resource "aws_instance" "example" {
  ami           = "ami-0c55b159cbfafe1f0"  # Specify the AMI ID of your desired EC2 instance image
  instance_type = "t2.micro"  # Set the instance type here (e.g., t2.micro, t2.small, etc.)

  tags = {
    Name = "ExampleInstance"  # Set the name tag for the instance here
  }
}
```

<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Terraform%20Language%20Basics%20%E2%80%93%20Configuration%20Syntax%2002.png" width="800" height="400" alt="Terraform Language Basics – Configuration Syntax 02">

<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Terraform%20Language%20Basics%20%E2%80%93%20Configuration%20Syntax%2002.png" width="800" height="400" alt="Terraform Language Basics – Configuration Syntax 03">


## Comments in Terraform
1. For Single Line Comments with ```#``` or ```//```
2. Multi-line comment ```/* --- */```

## Terraform Providers
<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Terraform%20Providers.png" width="800" height="400" alt="Terraform Providers">

# Connect AWS to Terraform

To follow this tutorial you will need:
* The Terraform CLI (1.2.0+) installed.
* The AWS CLI installed.
* AWS account and associated credentials that allow you to create resources.


To use your IAM credentials to authenticate the Terraform AWS provider, set the ```AWS_ACCESS_KEY_ID``` environment variable.

```tf
$export AWS_ACCESS_KEY_ID=
```

```tf
$export AWS_SECRET_ACCESS_KEY=
```

<img src="https://github.com/vaibhavkapase1302/Infrastructure-as-Code-Terraform/blob/main/Connect%20AWS%20to%20Terraform.png" width="600" height="400" alt="Connect AWS to Terraform">



