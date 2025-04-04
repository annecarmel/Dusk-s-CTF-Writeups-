# 🐱 HTB Starting Point - Meow

> Status: ✅ Completed  
> Difficulty: ⭐ Easy  
> Points: 🎯 10 XP  
> Date: April 4, 2025  
> Handle: `dusk`  

---

## 🧠 Objective
Gain access to the **Meow** machine and capture the user flag.

---

## 🖥️ Machine Info
- **Name:** Meow
- **IP Address:** `10.129.239.98`
- **Port(s):** 23/tcp (Telnet)

---

## 🔎 Nmap Scan

```bash
nmap -sV -sC 10.129.239.98

---

## Result:
PORT   STATE SERVICE VERSION
23/tcp open  telnet  Linux telnetd

---

## 📡 Service Enumeration (Telnet)
telnet 10.129.239.98

💡 No credentials needed
Once inside, you get a shell prompt.

---
```nginx
## 🏁 Capture the Flag
cat /flag.txt

---

## 🎉 Flag:
b40abdfe23665f766f9c61ecba8a4c19

---

## **🧠 What I Learned**
Basics of using telnet
Initial exposure to CTF walkthroughs
Setting up VPN & first access through HTB

---

## 💬 Notes by Dusk 🌘
Telnet is super outdated but still fun to poke at!
VPN config had to be fixed using OpenVPN and Admin PowerShell on Windows.
Had to enable Telnet manually using:
```bash
dism /online /Enable-Feature /FeatureName:TelnetClient

