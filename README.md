# Deploy_EC2_instance_with_Terraform

# Install Terraform on Linux


-  cd ~/

- wget
https:/ releases.hashicorp.com/terraform/0.13.4/terraform_0.13.4_linux_amd64.zip

- unzip terraform_0.13.4_linux_amd64.zip

- sudo mv terraform /usr/local/bin

1. **Configure Terraform providers**:

    provider “aws” {
        region = “us-east-1”
    }


1. **Create AWS resources with Terraform**:

    resource “aws_instance” myec2 {
        ami = “ami-0083662ba17882949
        instance_type = “t2.micro”
            tags = {
            “Name” = “Terraform_ec2”
            }
    }


