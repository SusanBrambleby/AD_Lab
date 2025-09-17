# AD_Lab
Active Directory Lab: Windows Server 2019 DC + Windows 10 client + GPO testing
# Active Directory Lab

## Overview
This lab demonstrates a Windows Server 2019 Domain Controller (DC) with a Windows 10 client. It includes:
- Active Directory setup
- Organizational Units (OUs)
- Users and Groups
- Group Policy Object (GPO) testing

## Lab Setup

1. **VMware Workstation Pro 17**  
2. **Windows Server 2019 ISO** → Domain Controller  
3. **Windows 10 ISO** → Client VM  
4. **Network:** Host-Only (VMnet1), DC IP: 192.168.31.10, Client IP: 192.168.31.11

## Screenshots

### 1. VM Overview
![VMs](screenshots/vms.png)

### 2. Active Directory Users and Computers
![ADUC](screenshots/aduc.png)

### 3. Test GPO Applied (Desktop Wallpaper)
![GPO](screenshots/gp.png)

### 4. Windows 10 Client Logged into Domain
![Client Login](screenshots/client-login.png)

### 5. Ping Test
![Ping](screenshots/ping.png)
