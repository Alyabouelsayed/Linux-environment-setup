# Linux Environment Setup

## Overview

This project documents my hands-on setup of an Ubuntu 26.04 LTS virtual machine using Oracle VirtualBox.

The goal of this lab was to build a Linux environment for learning and practicing IT support, system administration, troubleshooting, and networking concepts.

## Environment

- Hypervisor: Oracle VirtualBox
- Operating System: Ubuntu 26.04 LTS
- Virtual Disk: 40 GB
- Memory: 4 GB RAM
- Processors: 2
- Network: NAT
- Graphics Controller: VMSVGA

## Installation

The virtual machine was configured and Ubuntu 26.04 LTS was installed as the guest operating system.

After installation, I completed the initial Ubuntu setup, configured the user account, and verified that the system booted successfully.

## System Updates

After installation, I updated the system package information and installed available updates using:

`sudo apt update`

During the update process, some packages initially returned download errors from the Ubuntu mirror. I ran the update process again and verified that the packages were successfully configured.

## What I Practiced

- Creating and configuring a virtual machine
- Installing Ubuntu Linux
- Basic Linux system configuration
- Working with the terminal
- Updating packages with APT
- Reading and troubleshooting terminal errors
- Rebooting and verifying the system
- Working with VirtualBox networking and virtual hardware

## Result

Ubuntu 26.04 LTS is installed and running successfully inside Oracle VirtualBox.

This environment will be used for future Linux, networking, system administration, and IT support labs.
