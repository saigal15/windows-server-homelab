# 🏠 Windows Server 2022 Home Lab

## 📖 Project Overview

This project demonstrates the deployment of a Windows Server 2022 Home Lab designed to practice Windows Server administration in a small enterprise environment.

The lab includes the installation and configuration of Active Directory Domain Services (AD DS), DNS, DHCP and Group Policy. A Windows 11 client was joined to the domain to simulate a real corporate environment.

---

## 🎯 Objectives

- Deploy a Windows Server 2022 Domain Controller
- Configure Active Directory Domain Services
- Configure DNS
- Configure DHCP
- Create users and security groups
- Join a Windows 11 client to the domain
- Apply Group Policy Objects (GPO)

---

## 🖥️ Environment

| Component | Technology |
|-----------|------------|
| Server | Windows Server 2022 |
| Client | Windows 11 |
| Directory Service | Active Directory |
| DNS | Windows DNS |
| DHCP | Windows DHCP |
| Policies | Group Policy |
| Virtualization | VirtualBox |

---

## ⚙️ Implemented Services

### Active Directory
The server was promoted to a Domain Controller and configured with Active Directory Domain Services.

Implemented features:

- Installed Active Directory Domain Services
- Promoted the server as a Domain Controller
- Created Organizational Units (OU)
- Created users
- Created security groups

#### Screenshot

![Active Directory](screenshots/02-active-directory-users.png)

### DNS

Configured the DNS Server role to provide name resolution for the Active Directory domain.

Implemented:

- Installed DNS Server
- Configured Forward Lookup Zone
- Verified name resolution

#### Screenshot

![DNS Manager](screenshots/03-dns-manager.png)

### DHCP

Configured the DHCP Server role to automatically assign IP addresses to domain clients.

Implemented:

- Created a DHCP Scope
- Configured IP Address Range
- Configured Default Gateway
- Configured DNS Server
- Verified IP address assignment

#### Screenshot

#### DHCP Scope

![DHCP Scope](screenshots/04-dhcp-manager.png)

#### Active Lease

The Windows 11 client (PC01) successfully received its IP address automatically from the DHCP server.

![DHCP Lease](screenshots/05-dhcp-manager.png)

### Group Policy

Configured and deployed Group Policy Objects to manage user settings.

Implemented:

- Linked a custom GPO to the Human Resources OU
- Configured a mapped network drive (R:)
- Automatically deployed the shared drive to domain users

#### Screenshots

![GPO Linked to OU](screenshots/06-gpo-link.png)

![Drive Mapping Configuration](screenshots/07-gpo-drive-map.png)

![Mapped Drive on Windows 11 Client](screenshots/08-gpo-result.png)

### Windows 11 Client

- Joined Windows 11 to the domain
- Logged in with a domain user
- Verified network configuration

---

## 📚 Skills Demonstrated

- Windows Server Administration
- Active Directory
- DNS
- DHCP
- Group Policy
- User Management
- Domain Administration
- Windows Networking
- Troubleshooting

---

## 📸 Screenshots

Screenshots will be added soon.

---

## 👨‍💻 Author

Mommsen ILANSEGARIN
