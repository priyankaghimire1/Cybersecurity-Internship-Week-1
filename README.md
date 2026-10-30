# Cybersecurity-Internship-Week-1

# My Kali Linux VirtualBox Lab Setup

## Overview
I set up a Kali Linux virtual machine using Oracle VM VirtualBox. I configured it with 8GB of RAM, 5 CPUs, and a 25GB virtual hard drive to create a dedicated, isolated environment for my cybersecurity learning and practice.

## What I Did

### 1. I Configured the Virtual Machine Hardware
I created a new virtual machine and allocated specific resources to ensure it runs smoothly:
*   I assigned **8192 MB (8GB) of Base Memory (RAM)**.
*   I allocated **5 Processors** to the VM.
*   I set the display to **16 MB of Video Memory** using the **VMSVGA** graphics controller.
*   I attached a **25.00 GB SATA virtual hard disk** (VDI) to store the operating system.

### 2. I Installed Kali Linux
I mounted the Kali Linux ISO and booted the VM. From the boot menu, I selected **"Graphical Install"** to set up the operating system with a full desktop environment. I completed the installation process and rebooted the machine.

### 3. I Set Up the Network
To ensure my Kali machine has internet access while remaining isolated from my physical host, I configured the network settings:
*   In the VM settings, I attached **Adapter 1** to **NAT**.
*   In the VirtualBox global settings, I created a NAT Network called **"NatNetwork"**.
*   I set the IPv4 Prefix to **`10.0.2.0/24`** and enabled the DHCP server.

### 4. I Booted the System and Accessed the Terminal
Once the installation was complete, I logged into the Kali Linux desktop. I opened the terminal to start using the system. 

In the terminal, I am logged in as the user **`kali@Priyanka`**. My current working directory is **`/mnt/c/Users/priya`**, which indicates I am working within a mounted shared folder connected to my host machine's file system.

## Result
I now have a fully functional, isolated Kali Linux environment ready for security testing and learning.