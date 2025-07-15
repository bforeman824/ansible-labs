# Ansible Lab – Asset Inventory Collection

This lab demonstrates the use of Ansible to perform automated asset discovery and inventory collection across multiple EC2 instances.

## 🔧 Lab Overview

The `gather_assets.yml` playbook uses Ansible's built-in `setup` module to collect system facts (hostname, OS version, IP address, disk info, etc.) from remote hosts. It simulates a real-world Configuration Management scenario for managing and tracking infrastructure.

## 📂 File Structure

- `gather_assets.yml` – The main Ansible playbook used to collect system information
- `hosts.ini.example` – Sample Ansible inventory file with placeholder IPs (edit with your actual host details)
- `.gitignore` – Prevents accidental commits of sensitive files like your real `hosts.ini`

## 📋 Usage
1. **Clone the repository**:
   ```bash
   git clone https://github.com/<your-username>/ansible-labs.git
   ```

2. **Navigate to the asset inventory lab folder**:
   ```bash
   cd ansible-labs/02-asset-inventory
   ```

3. **Create your own `hosts.ini`** based on the provided example:
   ```bash
   cp hosts.ini.example hosts.ini
   ```

4. **Update `hosts.ini`** with your actual EC2 IP addresses and key path.

5. **Run the playbook**:
   ```bash
   ansible-playbook -i hosts.ini gather_assets.yml
   ```

## 🔐 Security Notice

This repo **does not include any real IP addresses or SSH keys**. The real `hosts.ini` file is excluded via `.gitignore`.

## ✍️ Author

Brianna Foreman  
Configuration Management | Network Automation | Ansible Labs  
