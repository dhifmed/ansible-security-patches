# Ansible Role: Apply Security Patches

This Ansible role applies security updates to both **Debian-based** (e.g., Ubuntu) and **RedHat-based** (e.g., RHEL, CentOS) systems. It also generates a security update log and backs up security-related log files.

## 🚀 Features

- Automatically updates APT cache for Debian-based systems.
- Installs and runs `unattended-upgrades` for security updates on Debian.
- Installs `yum-plugin-security` and applies security patches on older RedHat systems (RHEL/CentOS < 8).
- Creates a backup of system security log files.
- Gathers update details and generates a summary log using a template.
- Notifies handlers to reboot if required.

## 📁 Role Structure

This role assumes the following structure:

