# Cyber Security Training - Day 4

**Date:** 06 July 2026

---

## Introduction

On the fourth day of my Cyber Security training, I learned about Linux file permissions, file ownership, root and normal users, the `sudo` command, password management, and system updates. These concepts are essential for Linux administration and cybersecurity.

---

## Linux File Permissions

Linux uses three basic permissions to control access to files and directories.

| Permission | Symbol | Numeric Value | Description |
|------------|--------|---------------|-------------|
| Read | `r` | 4 | Allows viewing the contents of a file. |
| Write | `w` | 2 | Allows modifying or editing a file. |
| Execute | `x` | 1 | Allows executing a file or script. |

To check file permissions:

```bash
ls -l
```

---

## Changing File Permissions

The `chmod` command is used to modify file permissions.

### Numeric Method

```bash
chmod 110 hash.txt
```

Example:

```bash
chmod 440 hash.txt
```

Permission Breakdown:

- Owner: Read (`4`)
- Group: Read (`4`)
- Others: No Permission (`0`)

### Symbolic Method

```bash
chmod u+rwx filename
```

Where:

- `u` = User (Owner)
- `g` = Group
- `o` = Others
- `+` = Add permission
- `-` = Remove permission

Example:

```bash
chmod u+r hash.txt
```

---

## File Ownership

Every file in Linux has:

- Owner
- Group
- Others

To change the owner of a file:

```bash
sudo chown root hash.txt
```

To verify the changes:

```bash
ls -l
```

---

## Root User vs Normal User

Linux uses different symbols to represent different users.

| Symbol | User Type |
|--------|-----------|
| `#` | Root User |
| `$` | Normal User |

- The **Root User** has complete administrative privileges.
- The **Normal User** has limited permissions.

---

## The `sudo` Command

`sudo` stands for **Super User Do**.

It allows a normal user to execute commands with root privileges.

Examples:

```bash
sudo chmod 440 hash.txt
```

```bash
sudo chown root hash.txt
```

Whenever a permission error occurs, `sudo` can be used (if the user has permission) to execute the command.

---

## Changing the Root Password

To change the root password:

```bash
passwd root
```

If permission is denied:

```bash
sudo passwd root
```

After entering the new password twice, the password is updated successfully.

---

## Updating the System

To update the package list in Kali Linux:

```bash
sudo apt update
```

I learned that running `apt update` as a normal user may fail because administrative privileges are required.

---

## Commands Practiced

```bash
ls -l
chmod 110 hash.txt
chmod 440 hash.txt
chmod u+rwx filename
sudo chown root hash.txt
passwd root
sudo passwd root
sudo apt update
```

---

## Key Learning Outcomes

- Learned Linux file permissions (`r`, `w`, `x`).
- Understood numeric permission values (4, 2, 1).
- Practiced changing file permissions using the `chmod` command.
- Learned symbolic permission notation (`u`, `g`, `o`).
- Understood file ownership in Linux.
- Learned how to change file ownership using the `chown` command.
- Understood the difference between root and normal users.
- Learned the purpose and use of the `sudo` command.
- Practiced changing the root password.
- Learned how to update Kali Linux using `sudo apt update`.

---
