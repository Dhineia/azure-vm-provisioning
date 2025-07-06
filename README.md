# Azure VM Provisioning via Terraform

A simple Infrastructure-as-Code project to provision an Ubuntu-based virtual machine on Microsoft Azure using Terraform. This setup automates VM deployment, secures access via SSH, and includes manual installation of Nginx for basic web server functionality.

---

## Architecture Flow
![image](https://github.com/user-attachments/assets/7a01dc17-3159-4312-b718-35f35b93201a)
---

## Technologies Used

- Terraform – Infrastructure as Code to define and deploy Azure resources  
- Azure – Cloud provider used to host the VM  
- GitHub – Version control and source hosting  
- Nginx – Lightweight web server installed on the VM  
- SSH – Secure shell access to manage the virtual machine  

---

## Project Structure

| File             | Purpose                                              |
|------------------|------------------------------------------------------|
| `main.tf`        | Core Terraform configuration to define resources     |
| `variables.tf`   | Input variables for flexible deployment              |
| `outputs.tf`     | Output values like public IP                         |
| `terraform.tfvars` | Values assigned to input variables (optional)     |
| `README.md`      | Project overview and setup instructions              |

---

## How to Deploy

### 1. Clone the Repository

Bash
- git clone https://github.com/Dhineia/azure-vm-provisioning.git
- cd azure-vm-provisioning
- terraform init
- terraform plan
- terraform apply

---
## Install Nginx Inside the VM
- sudo apt update
- sudo apt install nginx -y
  
---

## Visit the site:
- http://<your_public_ip>
