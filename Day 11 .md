# Cyber Security Training – Daily Diary
## Day 11 – Firewall (UFW) and Common Network Ports
**Date:** 15/07/2026

### Objective
Today's session focused on understanding **Firewalls** in Linux using **UFW (Uncomplicated Firewall)**. The trainer explained how firewalls protect a system by allowing or blocking network traffic. We also learned about common network ports, protocols, and how to create firewall rules.

### Topics Covered

#### 1. Introduction to UFW (Uncomplicated Firewall)
UFW is a command-line utility used in Linux to configure and manage firewall rules in a simple way. It helps secure a system by controlling incoming and outgoing network connections.

#### 2. Basic UFW Commands

- Install UFW:
  ```bash
  sudo apt install ufw
  ```

- Check firewall status:
  ```bash
  sudo ufw status
  ```

- Enable the firewall:
  ```bash
  sudo ufw enable
  ```

- Reset the firewall (removes all configured rules):
  ```bash
  sudo ufw reset
  ```

**Note:** After resetting, the firewall automatically returns to an **inactive** state and must be enabled again if required.

#### 3. Default Firewall Policy

By default, UFW allows outgoing connections. This can also be configured using:

```bash
sudo ufw default allow outgoing
```

This means the system can initiate connections to other devices while incoming traffic is controlled according to firewall rules.

#### 4. Adding Firewall Rules

The trainer explained that firewall rules can be added in two ways:

- By **Port Number**
- By **Protocol/Service Name**

Example:

```bash
sudo ufw allow 22
```

or

```bash
sudo ufw allow ssh
```

Both commands allow SSH traffic through the firewall.

### Common Network Ports Learned

| Port | Protocol/Service | Purpose |
|------|------------------|---------|
| 21 | FTP | File Transfer Protocol |
| 22 | SSH | Secure Shell for remote login |
| 23 | Telnet | Remote access (less secure than SSH) |
| 25 | SMTP | Simple Mail Transfer Protocol (Email) |
| 53 | DNS | Domain Name System |
| 80 | HTTP | Web traffic |
| 139 | NetBIOS | Windows network communication |
| 443 | HTTPS | Secure web communication |
| 445 | SMB | Windows file sharing |
| 587 | Secure SMTP | Secure email submission |
| 2049 | NFS | Network File System |
| 3306 | MySQL | MySQL Database Server |
| 3389 | RDP | Remote Desktop Protocol |
| 5432 | PostgreSQL | PostgreSQL Database |
| 5900 | VNC | Virtual Network Computing (Remote Desktop) |

### Practical Commands Practiced

```bash
sudo apt install ufw
sudo ufw status
sudo ufw enable
sudo ufw reset
sudo ufw default allow outgoing
sudo ufw allow 22
sudo ufw allow ssh
sudo ufw allow 80
sudo ufw allow 443
```

### Key Learnings

- Learned the importance of firewalls in protecting computer systems.
- Understood how to install, enable, check, and reset UFW.
- Learned that firewall rules can be created using either port numbers or protocol names.
- Gained knowledge of commonly used network ports and their services.
- Understood the role of SSH, HTTP, HTTPS, DNS, SMTP, FTP, RDP, VNC, MySQL, PostgreSQL, and other networking protocols in cybersecurity.
- Performed basic firewall configuration commands for securing a Linux system.

### Conclusion

Today's practical session provided a solid introduction to Linux firewall management using UFW. I learned how firewall rules work, how to manage them through command-line commands, and became familiar with several important network ports and services that are commonly used in cybersecurity and system administration.
