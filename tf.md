## Infrastructure As Code - IaC  

- Infrastructure as code is the process of managing and provisioning computer data centers through machine-readable definition files **CODE**.
- Infrastructure as Code (or IaC) is an automated type of infrastructure management. The model approaches networks, virtual machines, storage etc in a descriptive manner via versioning (similar to DevOps tracking source code).
- Like Developers write Application Code to build Applications, Technologies - Java, Python, Node etc
- As a DevOps Engineer will be writing Infrastructure Code to build Infrastructure - AWS Cloudformation, Azure ARM, **Terraform** etc
- IaC boosts productivity through automation
- Consistency in Setup & Configuration by Minimising risk of human errors
- Replicate your infrastructure easily, CODE = REUSABILITY
- Makes your infrastructure Auditable, Since you can version control IaC configuration files like any source code file, you have full traceability of the changes

## Terraform

- Terraform is an Infrastructure As Code IaC software from HashiCorp.
- Terraform can build the infrastructure on cloud service providers such as AWS, Microsoft Azure or Google Cloud Platform etc
- Infrastructure is defined in HCL - Hashicorp Configuration Language

## Setup Terraform 

- https://developer.hashicorp.com/terraform/install
``` bash
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform
```