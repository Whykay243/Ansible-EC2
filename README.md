# Infrastructure Provisioning and Configuration Management with Ansible

## Project Overview

This project demonstrates infrastructure provisioning and configuration management using **Ansible** and **GitHub Actions** automation.

I provisioned several AWS EC2 instances, installing and configuring different services:
- Some servers run **Nginx**.
- Others run **Apache2** and **MySQL**.

The entire provisioning process is automated with GitHub Actions workflows, enabling continuous integration and deployment.

## Repository Structure

### 1. Infrastructure Provisioning Repository  
**[Ec2-Infra-provisioning-for-ANSIBLE (Public)](https://github.com/Whykay243/Ec2-Infra-provisionnig-for-ANSIBLE.git)**  
This repo contains the code to provision EC2 instances and install base services using automation.

### 2. Configuration Management Repository  
**[Ansible-EC2](https://github.com/Whykay243/Ansible-EC2.git)**  
This repo contains Ansible playbooks and configuration management files used to configure the provisioned servers.

Key contents include:
- `all.yml`: Defines all project variables.
- `inventory/host.ini`: Lists the IP addresses of Nginx servers, Apache2 servers, and MySQL database servers.
- `.github/workflows/`: Contains GitHub Actions CI/CD pipelines automating deployment.
- `playbook/files/`: Stores web homepage files for both Nginx and Apache servers.
- `playbook/`: Main Ansible playbooks referencing variables from `all.yml`.

## Security

Sensitive variables (e.g., credentials, API keys) are stored securely as **GitHub Actions secrets** to prevent exposure.

---

Feel free to explore the repositories and the automation workflows used to provision and configure a scalable web infrastructure on AWS using Ansible!
