 
🖥️Windows Server Enterprise Infrastructure Project

📌 Overview : 

       This project demonstrates the design and deployment of a small-to-medium enterprise Windows Server infrastructure using Microsoft technologies.
       The environment integrates Identity Management, Network Services, File Sharing, Security Policies, Storage, and Remote Access to simulate a real-world production domain following System Administration best practices.
       The objective is to build a secure, centralized, scalable, and manageable domain environment that supports multiple departments, controlled access, and reliable services.

🏗️Infrastructure Architecture:

🔹 Core Components

     Domain Layer
     
           Primary Domain Controller (Forest Root)
           Child Domain Controller
           Active Directory Domain Services
           Centralized authentication
           
     Client Layer
     
           Domain-joined workstations
           Department-based users
           Policy-controlled access
           
     Server Services
     
           DHCP Server
           File Server
           Group Policy Management
           RRAS + VPN
           Dynamic Storage (Spanned / Striped / Mirrored)

🎯 Project Goals
     The infrastructure was designed to achieve:
  
          ✅ Centralized identity management
          ✅ Department-based access control
          ✅ Automated IP assignment using DHCP
          ✅ Secure file sharing with NTFS permissions
          ✅ Policy enforcement using GPO
          ✅ Storage optimization & fault tolerance
          ✅ Delegated administration
          ✅ Multi-domain scalability
          ✅ Secure remote access via VPN

🔧 Implemented Technologies
     Active Directory

      Forest: ITISYSADMIN.com
      Child Domain: NEWGRC.ITISYSADMIN.com
      Organizational Units per department
      Users & security groups
      Delegation of control to department managers
      
🔹 Network Services

      DHCP scope (10.0.0.0/24)
      IP exclusions & reservations
      MAC filtering
      Automatic client configuration
      DHCP configuration backup
      
🔹 File Services
      
      Centralized shared folder
      Role-based permissions:
            HR → Read
            Sales → Modify
            IT → Full Control
      Disk quotas for selected users

🔹 Group Policy

      Hide local drives
      Corporate wallpaper
      Startup script execution
      Central configuration enforcement
      GPO backup & recovery

🔹 Security Controls

      Logon hour restrictions
      Device-based login control      
      Password policies    
      Least privilege model
      MAC-based device filtering
      
🔹 Remote Access

      RRAS configuration
      Secure VPN connections
      Encrypted external access

🔹 Storage

      Spanned volume → Capacity
      Striped volume → Performance
      Mirrored volume → Fault tolerance 
      Dynamic disks

🔐 Security Policies

     The following protections were enforced:

        Access Control
  
           Department-based permissions
           Delegated OU management
           Restricted login times
           Login from assigned PCs only
  
        Infrastructure Protection
  
           Centralized authentication
           Policy hardening via GPO
           Storage quotas
           Backup configurations

📡 Domain Strategy
 
         Structure
         ITISYSADMIN.com
            └── NEWGRC.ITISYSADMIN.com

      Benefits

            Scalability
            Replication
            Load distribution
            Administrative separation

🖥️ Server Roles

      Server	                Purpose
      Domain Controller	       Authentication & AD DS
      DHCP	                   IP distribution
      File                     Server	Shared storage
      RRAS	                   VPN & routing
      Child                    DC	Replication & redundancy
      
🚀 Skills Demonstrated

      This project demonstrates practical knowledge of:

            Active Directory Administration
            User & Group Management
            DHCP Deployment
            File Server Security
            Group Policy Management
            VPN & RRAS Configuration
            Storage Engineering
            Delegation & RBAC
            Enterprise Infrastructure Design
            Troubleshooting & Validation

📘 Conclusion

      This lab simulates a realistic enterprise Windows infrastructure and integrates multiple System Administration domains into a single scalable architecture.
      
      It focuses on:

      Centralization
      Seurity
      Automation
      Reliability
      
      The project provides hands-on experience equivalent to real-world deployment scenarios and serves as a strong foundation for System Administration / Windows Server Engineer roles.
