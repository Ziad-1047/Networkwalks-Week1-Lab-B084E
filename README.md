# 🛡️ Virtual Pentesting Lab Setup (Week 1)

## 📖 Description
This repository documents the setup of a virtualized cybersecurity lab environment built from scratch. Using Oracle VirtualBox and Kali Linux, the project demonstrates how to create an isolated NAT Network, configure IP addressing and DNS resolution, and verify internet connectivity. It also covers the critical pentesting practice of creating clean VM snapshots for safe, repeatable testing. This lab serves as the foundation for future penetration testing and vulnerability assessment exercises.

## ⚙️ Lab Specifications
* **Hypervisor:** Oracle VirtualBox v7.2.22
* **Operating System:** Kali Linux 2025.4
* **Network Type:** NAT Network
* **Subnet:** `10.0.0.0/24`
* **Gateway:** `10.0.0.1`

## 🚀 Setup Process

### 1. VirtualBox Installation
Successfully downloaded and installed Oracle VirtualBox on a Windows host.
![VirtualBox Installation](https://github.com/Ziad-1047/Networkwalks-Week1-Lab-B048E-/blob/main/1_vbox_d.png)
![VirtualBox Installation](https://github.com/Ziad-1047/Networkwalks-Week1-Lab-B048E-/blob/main/2_vbox_i.png)
### 2. Virtual Machine Provisioning
installed the official Kali Linux ISO and configured the virtual hardware for optimal performance.
![VirtualBox Installation](https://github.com/Ziad-1047/Networkwalks-Week1-Lab-B048E-/blob/main/4_kali_iso.png)
### 3. NAT Network Configuration
Created a private NAT Network to ensure the VM has internet access while remaining isolated from the host network. DHCP is enabled to automatically assign IP addresses.
![VirtualBox Installation](https://github.com/Ziad-1047/Networkwalks-Week1-Lab-B048E-/blob/main/3_nat_network.png)

### 4. Kali Linux Network Settings
Manually configured the Kali Linux wired connection to align with the NAT Network subnet, assigning a static IP and setting Google's DNS (`8.8.8.8`).
![VirtualBox Installation](https://github.com/Ziad-1047/Networkwalks-Week1-Lab-B048E-/blob/main/5_setup_kali_network.png)

### 5. Connectivity & DNS Testing
Ran a ping test against `google.com` to verify that both DNS resolution and outbound internet routing were functioning correctly through the NAT Network.
![VirtualBox Installation](https://github.com/Ziad-1047/Networkwalks-Week1-Lab-B048E-/blob/main/6_check.png)

### 6. Snapshot Creation
Created a clean snapshot named **"fresh install"**. This is a crucial step in pentesting, allowing me to instantly revert the VM to a pristine state if a test breaks the OS or installs malicious malware.
![VirtualBox Installation](https://github.com/Ziad-1047/Networkwalks-Week1-Lab-B048E-/blob/main/7_snapshot.png)

## 🧠 Key Learnings
* **Virtualization:** Understanding how hypervisors manage hardware resources.
* **Networking:** The difference between standard NAT and NAT Network in VirtualBox, IP configuration, and gateway routing.
* **Lab Hygiene:** The importance of snapshots for safe, repeatable penetration testing.

---
*Created as part of the Networkwalks Cybersecurity Internship (Batch B082).*
*Special thanks to Sir Waqas Karim (CCIE) and the NETWORKWALKS team.*
