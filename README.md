# Ansible Lab

Hands-on Ansible learning repository covering Linux automation, configuration management, infrastructure orchestration, and production-style Ansible concepts.

## Concepts Covered

* Inventory Management
* Ad-hoc Commands
* Playbooks
* Idempotency
* Variables and Facts
* Jinja2 Templating
* Loops and Conditionals
* Handlers
* Tags
* Register Variables
* set_fact
* Error Handling
* Blocks / Rescue / Always
* Ansible Vault
* Roles
* Templates
* group_vars and host_vars
* Variable Precedence
* Multi-host Orchestration

---

# Project Structure

```text
ansible-lab/
├── group_vars/
├── host_vars/
├── nginx_role/
├── templates/
├── hosts
├── multi_hosts
├── *.yml
├── secrets.example.yml
├── .gitignore
└── README.md
```

---

# Features Implemented

* Automated package installation
* Service management
* Dynamic configuration generation
* Multi-user creation with loops
* Conditional task execution
* Handler-based service restarts
* Vault-encrypted secrets handling
* Role-based project organization
* Multi-host inventory simulation
* Group-specific and host-specific variables
* Runtime variable creation using set_fact
* Error handling with block/rescue/always

---

# Example Commands

## Run Playbook

```bash
ansible-playbook -i hosts install_nginx.yml -K
```

## Run Tagged Tasks

```bash
ansible-playbook -i hosts tags.yml --tags install
```

## Run Vault Playbook

```bash
ansible-playbook -i hosts vault_playbook.yml --ask-vault-pass
```

## View Inventory

```bash
ansible-inventory -i multi_hosts --list
```

---

# Notes

* This repository is for learning and practicing Ansible concepts.
* `secrets.yml` is excluded using `.gitignore`.
* `secrets.example.yml` demonstrates expected secret structure safely.

---

# Learning Goals

This project focuses on understanding:

* Infrastructure as Code (IaC)
* Declarative Automation
* Configuration Management
* Reusable Infrastructure Design
* Multi-host Orchestration
* Production-style Ansible Practices
