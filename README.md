# Active Directory + File Share Lab

This project demonstrates a basic **Windows Server 2019 Active Directory Domain Controller** setup with **Windows 10 clients**, including:
- Active Directory Users and Computers (ADUC) management
- File Share permissions with NTFS and Share Security
- Group Policy Object (GPO) application

---

## ⚙️ Lab Setup
- **Domain Controller:** Windows Server 2019 (DC01)
- **Client:** Windows 10 (Client)
- **Domain:** lab.local

---

## 👤 Active Directory
Created two OUs:
- `HR_OU`
- `IT_OU`

Users:
- `hr_user1` in `HR_OU`
- `it_user1` in `IT_OU`

📸 Screenshots:
- ![ADUC Users] (AD_Lab/ADUC with OUs,groups.png)
- ![ADUC Computers](screenshots/02-ADUC-Computers.png)

---

## 📂 File Shares
Created two shared folders on the DC:
- `HR_Files` → accessible only to `HR_Group`
- `IT_Files` → accessible only to `IT_Group`

📸 Screenshots:
- ![HR Share](screenshots/03-Share-HR.png)
- ![IT Share](screenshots/04-Share-IT.png)

---

## 🔑 Access Control Testing
- ✅ `hr_user1` → Access to HR_Files  
- ❌ `hr_user1` → Denied from IT_Files  
- ✅ `it_user1` → Access to IT_Files  

📸 Screenshots:
- ![HR Access](screenshots/05-Client-HR_Access.png)
- ![HR Denied IT](screenshots/06-Client-HR_Denied.png)
- ![IT Access](screenshots/07-Client-IT_Access.png)

---

## 🖥️ Group Policy
Created a test GPO `TestPolicy` linked to `HR_OU`.  
Policy: Set custom desktop wallpaper.

📸 Screenshots:
GPO Linked](screenshots/08-GPO-Linked.png)
[GPO Applied](screenshots/09-GPO-Result.png)
