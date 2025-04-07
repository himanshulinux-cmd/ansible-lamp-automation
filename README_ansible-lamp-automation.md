
# Ansible LAMP Stack Automation

Automates the provisioning and configuration of a LAMP (Linux, Apache, MySQL, PHP) stack across multiple Linux servers using Ansible.

## 📌 Tech Stack
- Ansible
- YAML
- Apache2, MySQL, PHP
- Linux (Ubuntu/CentOS)

## 🔧 Features
- Role-based Ansible playbooks
- Custom handlers and templates for Apache & PHP
- Firewall (iptables/ufw) & SELinux automation
- Inventory file with groups for web & db servers

## 🏗️ Architecture
```bash
[ Control Node (Ansible) ]
        |
-----------------------------
|           |             |
Web1       Web2         DB1
```

## 🚀 How to Run
1. Clone repo and update inventory.yaml
2. Modify group_vars/webservers and dbservers
3. Run:
```bash
ansible-playbook site.yml -i inventory.yaml
```

## 📂 Folder Structure
```
roles/
├── apache/
├── mysql/
├── php/
├── firewall/
inventory.yaml
site.yml
```

## 📈 Outcome
- Zero-touch LAMP deployment on new Linux servers within minutes.
- Easily scalable for future projects.
