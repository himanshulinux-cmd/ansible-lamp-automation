# Ansible LAMP Stack Automation

A fully automated deployment of the LAMP stack using Ansible, designed for multi-server environments to streamline web infrastructure provisioning.

## 🔧 Tech Stack
- Ansible
- Apache (HTTPD)
- MySQL
- PHP
- CentOS / RHEL / Ubuntu
- Bash scripting

## 📁 Folder Structure
- `/roles/` – Modular Ansible roles for Apache, MySQL, PHP, Firewall, and Users
- `/inventory.ini` – Inventory file for defining target hosts
- `/site.yml` – Master playbook to execute roles
- `/scripts/` – Supporting shell scripts (if any)

## 🚀 Key Features
- One-click deployment of LAMP stack
- Configurable through inventory and variables
- Clean role-based architecture for scalability
- Secure user and firewall setup included

## 🤖 How to Use
1. Clone the repo
2. Update `inventory.ini` with your target server(s)
3. Run the playbook:
   ```bash
   ansible-playbook site.yml -i inventory.ini
