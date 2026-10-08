# 🐧 Ubuntu Linux Virtualization & System Administration Lab

## 📌 Overview
This project documents the provisioning, deployment, and baseline configuration of an **Ubuntu 26.04 LTS** server/desktop environment inside an **Oracle VirtualBox** hypervisor. It demonstrates hands-on skills in virtual hardware allocation, Linux system setup, command-line interface (CLI) administration, package repository management, and basic Linux troubleshooting.

---

## 🛠️ System Architecture & Specifications
* **Hypervisor:** Oracle VirtualBox
* **Guest OS:** Ubuntu 26.04 LTS (x86_64)
* **Virtual Storage:** 40 GB Dynamically Allocated VDI
* **Memory (RAM):** 4 GB Allocated
* **CPU Allocation:** 2 vCPUs
* **Network Adapter:** NAT (Network Address Translation)
* **Graphics Controller:** VMSVGA (with VirtualBox Guest Additions)

---

## 🎯 Lab Objectives
* **Virtual Machine Provisioning:** Allocate and configure hardware resources optimized for Ubuntu 26.04 LTS.
* **Linux OS Installation:** Complete the clean installation and initial user setup wizard.
* **CLI & Package Management:** Utilize `apt` package manager to update repository indexes and upgrade system components.
* **System Diagnostics:** Analyze and resolve APT package mirror fetch errors during initial updates.

---

## 📑 Step-by-Step Implementation Guide

### Phase 1: Virtual Machine Creation & Resource Allocation
1. Created a new 64-bit Linux virtual machine instance in **Oracle VirtualBox**.
2. Configured CPU cores (2 vCPUs), system memory (4 GB RAM), and dynamic virtual disk storage (40 GB).
3. Attached the **Ubuntu 26.04 LTS ISO** image to the virtual optical drive and configured boot priority.

### Phase 2: OS Installation & Base Setup
1. Booted into the Ubuntu installer and initialized system installation.
2. Formatted virtual disk partitions and created the administrative root/sudo user account.
3. Completed initial system reboot and verified display driver resolution via VMSVGA driver configuration.

### Phase 3: CLI Administration & APT Troubleshooting
1. Opened the Linux terminal (`bash`) to execute system maintenance commands.
2. Executed package update index command:
   ```bash
   sudo apt update && sudo apt upgrade -y
2.
Troubleshooting Mirror Errors:
Encountered temporary package fetch failures ( 404 / Hash Sum mismatch) from regional Ubuntu archive mirrors.
Resolution: Verified outbound network connectivity via VirtualBox NAT interface, re-synchronized APT cache sources ( sudo apt update --fix-missing), and successfully completed all pending package upgrades.
• Key Skills Demonstrated
O
Virtualization Management: Hypervisor resource planning, virtual disk management, and guest additions optimization.
Linux CLI Proficiency: Terminal navigation, package management ( apt ), and user privilege management ( sudo).
Technical Troubleshooting: Reading CLI error logs, resolving package dependency/ mirror errors, and verifying system state post-reboot.

Future Enhancements
Networking: Switch network adapter from
NAT to Bridged Networking for local network visibility.
SSH & Remote Management: Install and configure openssh-server for remote CLI management and key-based authentication.
Automation: Writing Bash scripts to automate routine system maintenance and log rotation.
   
