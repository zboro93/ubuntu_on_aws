## ubuntu_on_aws
task3 - build Ubuntu instance with Terraform
---

**About**

My path to DevOps role.
As preparation and learning to be a DevOps Engineer, I began to perform practical tasks that will help and document my development.  
This task is to build Ubuntu EC2 instance on AWS, with all required infrastructure using Terraform.

---

**Build with**
 - Terraform
 - AWS 

---

**How it works**

Terraform file containe resources to build VCP, public subnet, security group with ingress rule for SSH port 22, internet gateway, route table, EC2 Ubuntu instance with public IP, key pair for SSH connection.

---

**Usage**

1. Copy Terraform file
    - copy main.tf to the destination folder
2. Source AWS credentials manully
    - export AWS_ACCESS_KEY_ID=
    - export AWS_SECRET_ACCESS_KEY=
3. Initialize Terraform
    - Terraform init
4. Apply Terraform main.tf
    - Terraform apply
5. Change permission for .pem file
    - chmod 600 MyAWSKey.pem
6. Connect to Ubuntu instance
    - ssh -i MyAWSKey.pem ubuntu@<ubuntu_public_ip>

---
