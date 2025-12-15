# 🔥 Task 4: Setup and Use a Firewall on Linux 🛡️

![Linux](https://img.shields.io/badge/OS-Linux-blue?style=for-the-badge)
![Kali](https://img.shields.io/badge/Distro-Kali%20Linux-lightblue?style=for-the-badge)
![UFW](https://img.shields.io/badge/Firewall-UFW-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

---

## 🎯 Objective
To **configure and test basic firewall rules** on a Linux system in order to **allow or block network traffic**, improving system security.

---

## 🛠️ Tools & Environment
- 🐧 **Operating System:** Kali Linux  
- 🔐 **Firewall Tool:** UFW (Uncomplicated Firewall)  
- 💻 **Platform:** VirtualBox  

---

## 📌 Task Description
In this task, a firewall was configured using **UFW** on Kali Linux.  
Inbound traffic on **port 23 (Telnet)** was blocked and tested to verify the rule.  
**SSH traffic (port 22)** was explicitly allowed to ensure secure remote access.  
Finally, the test rule was removed to restore the firewall to its original state.

---

## ⚙️ Steps Performed
✅ Installed UFW firewall  
✅ Enabled and verified firewall status  
✅ Listed existing firewall rules  
✅ Blocked inbound traffic on **port 23 (Telnet)**  
✅ Tested blocked port using `telnet`  
✅ Allowed **SSH (port 22)** traffic  
✅ Removed test rule and verified final configuration  

---

## 💻 Commands Used
```bash
sudo apt install ufw
sudo ufw enable
sudo ufw status
sudo ufw deny 23/tcp
telnet localhost 23
sudo ufw allow 22/tcp
sudo ufw delete deny 23/tcp
