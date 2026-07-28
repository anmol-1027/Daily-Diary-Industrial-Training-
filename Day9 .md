# Day 9 – Introduction to Penetration Testing and Port Scanning

**Date:** 13-07-2026

## Objective
The objective of today's session was to understand different cybersecurity job roles, learn the basics of penetration testing, identify the IP address of a target machine, and perform initial network reconnaissance using Metasploitable.

## Topics Covered

### 1. Cybersecurity Roles
We discussed some of the major roles in the cybersecurity field:

- **Penetration Tester (Ethical Hacker):**
  - Performs authorized attacks on systems.
  - Identifies vulnerabilities and security weaknesses before attackers can exploit them.

- **Security Analyst:**
  - Monitors and analyzes network infrastructure.
  - Detects suspicious activities and responds to security incidents.

- **Cybersecurity Engineer:**
  - Designs, implements, and maintains secure networks and systems.
  - Protects organizational infrastructure from cyber threats.

---

### 2. Working with Metasploitable

Today's practical session focused on **Metasploitable**, a deliberately vulnerable virtual machine used for cybersecurity training.

The instructor demonstrated how to:

- Start the Metasploitable virtual machine.
- Find the IP address of the target system using:

```bash
ifconfig
```

The IP address obtained was:

```
192.168.112.129
```

This IP address was later used as the target machine for security testing from Kali Linux.

---

### 3. Port Scanning

We learned the concept of **port scanning**, which is used to discover open ports and services running on a target system.

Key points covered:

- A computer contains **65,535 ports**.
- Port scanning helps identify which ports are open.
- Open ports may expose services that can be analyzed for vulnerabilities.
- Port scanning is one of the first steps in penetration testing.

---

## Commands Practiced

```bash
ifconfig
```

---

## Key Learnings

- Understood the responsibilities of different cybersecurity professionals.
- Learned the purpose of penetration testing.
- Identified the IP address of a vulnerable machine using `ifconfig`.
- Understood the importance of port scanning during reconnaissance.
- Learned that computers have **65,535 ports**, and scanning helps identify active services.

---

## Conclusion

Today's session introduced the fundamentals of penetration testing and network reconnaissance. We explored cybersecurity career roles, worked with the Metasploitable vulnerable machine, learned how to obtain its IP address, and understood the importance of port scanning as the first step in identifying potential security vulnerabilities.
