# Ansible NTP Lab

This lab demonstrates how to use Ansible to automate a basic configuration management task: installing and enabling the NTP (Network Time Protocol) service on a Linux system.

## 🔧 Files
- `hosts.ini`: Static inventory targeting localhost
- `ntp_setup.yml`: Ansible playbook that installs NTP and ensures the service is running
- Tested in a local Ubuntu-based virtual machine

## 🚀 Usage
```bash
ansible-playbook -i hosts.ini ntp_setup.yml
