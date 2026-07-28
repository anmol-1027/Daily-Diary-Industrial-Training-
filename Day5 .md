# Cyber Security Training - Day 5

**Date:** 07 July 2026

## Objective

The objective of today's session was to understand Linux user and group management, learn about important system files related to user accounts, practice creating users and groups, assign users to groups, and understand the Linux directory structure.

---

## Topics Covered

### 1. Linux User Information Files

Learned about the important files located in the `/etc` directory that store user and group information.

- **/etc/passwd**
  - Stores basic information about all user accounts.
  - Contains username, User ID (UID), Group ID (GID), home directory, and default shell.

- **/etc/shadow**
  - Stores encrypted passwords of users.
  - Accessible only by the root user for security purposes.

- **/etc/group**
  - Stores information about all groups available on the system.

- **/etc/gshadow**
  - Stores secure group password information and group administration details.

---

### 2. Creating a New User

Learned how to create a new user account in Linux.

**Command:**

```bash
sudo adduser user1
```

During user creation, Linux prompts for:

- Password
- User details (optional)
- Confirmation of the information

---

### 3. Viewing User Details

Learned how to display information about a user.

**Command:**

```bash
id user1
```

This command displays:

- User ID (UID)
- Group ID (GID)
- Groups the user belongs to

---

### 4. Creating a New Group

Learned how to create a new group to organize users and manage permissions.

**Command:**

```bash
sudo groupadd developers
```

Groups help in assigning common permissions to multiple users.

---

### 5. Adding a User to a Group

Learned how to associate (link) a user with an existing group.

**Command:**

```bash
sudo usermod -aG developers user1
```

The `-aG` option adds the user to the specified group without removing them from their existing groups.

To verify the group membership:

```bash
groups user1
```

or

```bash
id user1
```

---

### 6. Login Using Password

Learned how users log in to the Linux system using their username and password.

The authentication process checks the encrypted password stored in the `/etc/shadow` file before granting access to the system.

To switch to another user:

```bash
su - user1
```

The system prompts for the user's password before allowing login.

---

## Commands Practiced

```bash
cat /etc/passwd
cat /etc/shadow
cat /etc/group
cat /etc/gshadow

sudo adduser user1
id user1

sudo groupadd developers

sudo usermod -aG developers user1

groups user1

su - user1
```

---

## Learning Outcome

By the end of Day 5, I gained a clear understanding of Linux user and group management. I learned the purpose of important system files such as `/etc/passwd`, `/etc/shadow`, `/etc/group`, and `/etc/gshadow`. I practiced creating users and groups, linking users to groups, viewing user information, and logging into the system using passwords.
