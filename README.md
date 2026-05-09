# azure-remote-vm-management
# Azure Remote VM Management Project

## Overview
This project demonstrates secure remote access and management of Microsoft Azure Virtual Machines using Remote Desktop Protocol (RDP) for Windows and powershell terminal (SSH) for Linux.

The project also covers Network Security Group (NSG) configuration, public IP identification, and secure inbound access restrictions.

---

## Project Goals
- Configure Azure VM networking and security
- Connect remotely to Windows and Linux virtual machines
- Implement NSG security rules
- Restrict inbound access to authorized IP addresses
- Verify VM accessibility
- Demonstrate secure session management

---

## Technologies Used
- Microsoft Azure
- Windows Server 2022
- Ubuntu 22.04 LTS
- Remote Desktop Protocol (RDP)
- Secure Shell (SSH)
- Network Security Groups (NSG)

---

## Windows VM Connection (RDP)

### Steps
1. Created a Windows Server VM in Azure
2. Enabled inbound port 3389
3. Retrieved the public IP address
4. Connected using Remote Desktop Connection

### Verification
Successfully logged into the Windows Server desktop environment.

---

## Linux VM Connection (SSH)

### Steps
1. Created an Ubuntu Linux VM
2. Enabled inbound port 22
3. Retrieved the public IP address
4. Connected using SSH through terminal

### SSH Command Used

```bash
ssh felixchimaa@20.224.137.255
```

### Verification
Successfully accessed the Linux command-line environment and executed system commands.

---

## NSG Configuration

### Windows VM Rule
| Port | Protocol | Access |
|---|---|---|
| 3389 | TCP | Allow |

### Linux VM Rule
| Port | Protocol | Access |
|---|---|---|
| 22 | TCP | Allow |

### Security Improvement
Inbound rules were restricted to a specific source IP address using the “My IP” option in Azure NSG settings.

---


## Conclusion
This project provided practical experience with Azure networking, remote VM administration, and cloud security best practices using RDP and SSH protocols.
