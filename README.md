# AyoLab-Active-Directory-Project
A self-initiated enterprise IT environment built from scratch to simulate real-world systems administration. This project demonstrates the design and deployment of a Windows Server 2019 domain (Ayolab.lab) integrated with Active Directory (AD DS), DNS, Group Policy, file services (SMB), and GLPI IT Service Management (ITSM) via LDAP synchronization


# 🧬 AyoLab Active Directory & Infrastructure Project

**Author:** Ayodele Fadoju  
**Tech Stack:** Windows Server 2019 | Active Directory | DNS | GPO | SMB | GLPI | PowerShell | VirtualBox  
**Location:** Ontario, Canada  

---

## 🌍 Project Overview

**AyoLab** is a self-initiated enterprise IT infrastructure project that demonstrates how real-world organizations manage identity, security, and automation using Microsoft technologies.  

Named after its creator — *“Ayo”* — AyoLab was built entirely from the ground up to simulate a biotech startup with over 50 employees across seven departments. The environment integrates **Active Directory (AD DS)**, **DNS**, **Group Policy**, **file services (SMB)**, and **GLPI (ITSM)** — fully automated through **PowerShell scripting**.  

This project showcases my ability to plan, deploy, and document enterprise systems that reflect production-grade standards in IT administration, automation, and support.

---

## 🧩 Problem Statement

AyoLab, a fictional biotech research company funded by the United Nations, was preparing to scale operations but lacked a structured IT environment.  

The organization faced:
- Disconnected user accounts with no centralized identity system  
- Unsecured file sharing and inconsistent access permissions  
- No IT helpdesk or system visibility  
- Manual provisioning that slowed operations and created security gaps  

These challenges made collaboration inefficient and increased the risk of compliance and data management issues — critical concerns in a biotech environment.

---

## 💡 Solution Overview

To address these issues, I designed and deployed a **Windows Server 2019 domain environment (`Ayolab.lab`)** with centralized identity, policy enforcement, file management, and integrated IT service support.  

The solution included:
- **Active Directory (AD DS)** for centralized user authentication  
- **DNS** for name resolution and domain management  
- **Group Policy Objects (GPOs)** for enforcing security and configuration standards  
- **PowerShell automation** for user, OU, and group provisioning  
- **SMB file shares** with NTFS-based permissions for departmental security  
- **GLPI ITSM** integration via LDAP for helpdesk and asset management  

All configurations were documented, scripted, and validated inside a **VirtualBox lab** simulating seven functional departments: Executive, R&D, IT, HR, Sales, Compliance, and LabOps.

---

## ⚙️ Implementation Summary

### **1. Environment Setup**
- Installed **Windows Server 2019** and configured roles for **AD DS** and **DNS**.  
- Promoted the server to a new forest: `Ayolab.lab`.  
- Deployed a **Windows 11 client** joined to the same domain.

### **2. Active Directory Configuration**
- Created Organizational Units (OUs) for each department.  
- Automated OU creation using the PowerShell script `New-AyoLab-OUs.ps1`.  
- Imported 50+ users from CSV using `Import-AyoLab-Users.ps1`.  

### **3. File and Access Services**
- Created departmental SMB shares using `New-AyoLab-Shares.ps1`.  
- Applied NTFS and share permissions per OU to ensure secure collaboration.  

### **4. Policy Enforcement**
- Designed baseline Group Policies for password policies, updates, and mapped drives.  
- Backed up and versioned policies using `Backup-GPOs.ps1`.  

### **5. ITSM Integration**
- Installed **GLPI** using XAMPP and connected it to Active Directory via LDAP.  
- Created user profiles, roles, and entities to mirror the domain structure.  
- Tested authentication, asset inventory, and ticket routing.

### **6. Validation**
- Verified domain logins, GPO applications, DNS resolution, and GLPI connectivity.  
- Documented procedures for reproducibility and portfolio demonstration.

---

## 🧠 Skills and Technologies Used

| Category | Tools / Technologies | Description |
|-----------|----------------------|--------------|
| **System Administration** | Windows Server 2019, AD DS, DNS, GPO | Centralized authentication and domain management |
| **Automation** | PowerShell | User creation, OU setup, and GPO backup automation |
| **Networking** | NAT + Bridged (VirtualBox) | Network connectivity between DC and client |
| **File Services** | SMB, NTFS Permissions | Department-based access control |
| **ITSM** | GLPI + LDAP | Centralized ticketing and asset management |
| **Documentation & Control** | GitHub, Markdown | Clear, reproducible technical documentation |

---

## 🌙 Challenges & Lessons Learned

This project demanded **months of troubleshooting, research, and late nights** configuring PowerShell scripts, DNS records, and GPOs that refused to cooperate.  

Every setback taught me:
- **Resilience** — to keep testing until the environment worked  
- **Patience** — to understand each service deeply, not just follow steps  
- **Perseverance** — because real-world IT is built on continuous learning  

> “You don’t learn IT by reading manuals; you learn it by breaking things, fixing them, and refusing to give up.”

---

## 🏁 Results

- Centralized and secure domain infrastructure (`Ayolab.lab`)  
- Fully automated provisioning and configuration with PowerShell  
- Departmental file shares and enforced GPO security policies  
- GLPI ITSM system connected to AD via LDAP  
- Scalable documentation for reproducibility and portfolio display  

This project demonstrates my readiness to manage **Microsoft 365**, **Active Directory**, and **cloud-integrated systems** with structure, automation, and clarity.

---

## 🚀 Future Enhancements

- Integrate **Active Directory Certificate Services (AD CS)**  
- Deploy **WSUS** for patch management  
- Configure **Azure AD Connect** for hybrid identity sync  
- Add **monitoring dashboards** (Grafana + WMI) for server health metrics  

---

## 👤 Author

**Ayodele Fadoju**  
🎓 Cloud Data Management | Conestoga College  
💼 Microsoft 365 & Systems Administration | IT Infrastructure | Automation  
🔗 [LinkedIn](https://www.linkedin.com/in/fadojuayodele/)  
📧 fadojuayodeleolafimihan@gmail.com  

> *“Technology is more than code — it’s about designing systems that empower people to work smarter and securely.”*

---

## 📝 License

This project is released under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.
