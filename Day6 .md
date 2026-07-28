# Cyber Security Training - Day 6

**Date:** 08 July 2026

## Objective

The objective of today's session was to learn how to configure sudo permissions in Linux, understand the structure of the `sudoers` file, assign command-specific privileges to users and groups, and practice user and group management through a hands-on task.

---

## Topics Covered

### 1. Introduction to Sudo Configuration

Learned about the purpose of **sudo (Super User Do)** and how it allows normal users to execute administrative commands without logging in as the root user.

---

### 2. Editing the Sudoers File

Learned how to safely edit the sudo configuration file using the `visudo` command.

**Command:**

```bash
visudo
```

The `visudo` command opens the sudoers file in a safe editing mode and checks for syntax errors before saving the file.

---

### 3. Sudoers Configuration File

Learned about the sudo configuration file:

```text
/etc/sudoers
```

This file defines which users or groups are allowed to execute administrative commands.

---

### 4. Understanding Sudoers Syntax

Learned the meaning of the following rule:

```text
user ALL=(ALL:ALL) ALL
```

Explanation:

- **user** → Username that receives the permission.
- **First ALL** → The systems or hosts where the rule applies.
- **(ALL:ALL)** → The user and group privileges that can be assumed.
- **Last ALL** → The commands that the user is allowed to execute.

Also learned that:

- When defining permissions for a **user**, the username is written directly.
- When defining permissions for a **group**, the group name is written with a `%` symbol.

Example:

```text
%class ALL=(ALL:ALL) ALL
```

---

### 5. Finding the Location of Commands

Learned how to find the absolute path of a command using:

```bash
which command
```

Example:

```bash
which apt
```

This command displays the full path of the executable, which is useful when granting permission for specific commands in the sudoers file.

---

## Practical Task

Performed a hands-on lab to practice user and group management.

### Task Steps

1. Created a new user using my own name.
2. Created a new group named **class**.
3. Added my user account to the **class** group.
4. Modified the sudoers file using `visudo`.
5. Granted permission to execute only the following command using sudo:

```bash
sudo apt
```

This demonstrated how to provide limited administrative privileges instead of giving full root access.

---

## Commands Practiced

```bash
adduser Apram

groupadd class

usermod -aG class Apram

id Apram

groups Apram

visudo

which apt
```

---

## Learning Outcome

By the end of Day 6, I understood how Linux manages sudo privileges using the `/etc/sudoers` file. I learned how to safely edit the sudoers configuration with `visudo`, interpret sudo permission rules, locate command paths using `which`, create users and groups, link users with groups, and grant permission to execute specific administrative commands. This session helped me understand the principle of least privilege by allowing only selected commands instead of full administrative access.
