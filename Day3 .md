# Cyber Security Training - Day 3

**Date:** 03 July 2026

---

# Introduction

On the third day of my Cyber Security training, I learned about the Linux Directory Structure. The trainer explained how Linux organizes files and directories in a hierarchical structure, making it easier to manage the operating system efficiently. I also practiced basic directory navigation commands to understand how users interact with the Linux file system.

---

# Linux Directory Structure

Linux follows a hierarchical file system that begins from the **root directory (`/`)**. Every file and directory in Linux is stored under this root directory.

```
/
├── bin
├── boot
├── dev
├── etc
├── home
├── lib
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin
├── srv
├── sys
├── tmp
├── usr
└── var
```

---

# Important Linux Directories

## `/` (Root Directory)

The root directory is the top-level directory of the Linux file system. Every other directory is located under this directory.

---

## `/home`

The `/home` directory contains personal files and folders of normal users.

Example:

```bash
/home/kali
```

---

## `/root`

The `/root` directory is the home directory of the root (administrator) user.

---

## `/bin`

The `/bin` directory stores essential command-line programs that are required for basic system operations.

Examples:

- `ls`
- `cp`
- `mv`
- `cat`
- `pwd`

---

## `/sbin`

The `/sbin` directory contains system administration commands that are mainly used by the root user.

---

## `/etc`

The `/etc` directory stores system configuration files.

Examples include:

- Network configuration
- User account information
- Service configuration files

---

## `/usr`

The `/usr` directory contains installed applications, libraries, documentation, and user utilities.

---

## `/var`

The `/var` directory stores variable data such as:

- Log files
- Cache files
- Mail files

---

## `/tmp`

The `/tmp` directory stores temporary files created by applications and the operating system.

---

## `/dev`

The `/dev` directory contains device files representing hardware devices connected to the system.

---

## `/proc`

The `/proc` directory is a virtual file system that provides information about running processes and the Linux kernel.

---

## `/boot`

The `/boot` directory contains files required to start the Linux operating system.

---

## `/opt`

The `/opt` directory is used to install optional or third-party software packages.

---

# Basic Commands Practiced

```bash
pwd
ls
cd
cd ..
cd /
cd ~
```

---

# Why Directory Structure is Important

- Organizes files and folders efficiently.
- Makes file navigation easier.
- Separates system files from user files.
- Improves system management and security.
- Helps administrators locate important files quickly.
- Supports multiple users by providing separate home directories.

---

# Key Learning Outcomes

- Understood the Linux directory hierarchy.
- Learned the purpose of the root directory (`/`).
- Identified the functions of important Linux directories.
- Learned where user files, system files, applications, and logs are stored.
- Practiced navigating directories using Linux commands.
- Understood the importance of the Linux file system in cybersecurity.

---

# Conclusion

Day 3 focused on understanding the Linux Directory Structure and its importance in the Linux operating system. I learned how files are organized, the purpose of major system directories, and how to navigate through the file system using basic Linux commands. This knowledge forms the foundation for Linux administration and future cybersecurity tasks.
