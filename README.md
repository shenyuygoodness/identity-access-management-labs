# identity-access-management-labs
Hands-on Li# 🛡️ Identity and Access Management (IAM) Labs

## 📌 Overview

This repository contains hands-on practical labs for the **Identity and Access Management (IAM)** course.
The labs focus on implementing security concepts in Linux systems, including user management, access control, authentication, and system protection mechanisms.

These exercises were performed using multiple Linux distributions such as **Kali Linux, Ubuntu, and CentOS/AlmaLinux**.

---

## 👤 Student Information

* **Name:** Shenyuy Goodness-Divine Tata
* **Matricule:** UBa25EP116
* **Course:** Identity and Access Management (IAM)

---

## 🧪 Labs Covered

This project includes **Lab 1 to Lab 12**:

### 🔹 Lab 1: Assigning Limited Sudo Privileges

* Created multiple users
* Configured `/etc/sudoers` using `visudo`
* Implemented role-based access control

---

### 🔹 Lab 2: Disabling the Sudo Timer

* Used `sudo -k` to reset authentication
* Configured `timestamp_timeout` in sudoers
* Applied user-specific timeout policies

---

### 🔹 Lab 3: Encrypted Home Directory

* Installed encryption tools
* Created a user with encrypted home directory
* Verified encryption behavior

---

### 🔹 Lab 4: Password Complexity Policy

* Configured password rules in `pwquality.conf`
* Enforced strong password requirements
* Tested weak vs strong passwords

---

### 🔹 Lab 5: Account & Password Expiry

* Managed account expiration dates
* Configured password aging using `chage`
* Forced password reset on first login

---

### 🔹 Lab 6: Detecting Compromised Passwords

* Used `curl` with the Have I Been Pwned API
* Executed password-checking script
* Identified compromised passwords

---

### 🔹 Lab 7: Account Lockout with PAM

* Configured login attempt limits using `pam_tally2`
* Locked accounts after failed attempts
* Reset account access

---

### 🔹 Lab 8: Distributed Identity Management

* Installed **FreeIPA** and **Adsys**
* Explored centralized authentication systems

---

### 🔹 Lab 9: SUID & SGID Files

* Scanned system for SUID/SGID files
* Identified potential privilege escalation risks

---

### 🔹 Lab 10: File Attributes (chattr)

* Applied `+a` (append-only) and `+i` (immutable)
* Tested file protection behavior

---

### 🔹 Lab 11: Shared Group Directory

* Created a shared directory using groups
* Applied permissions (`chmod 3770`)
* Used **SGID** and **sticky bit**
* Configured **ACL** for fine-grained access control

---

### 🔹 Lab 12: SELinux Type Enforcement

* Configured Apache web server
* Tested SELinux file context restrictions
* Demonstrated access denial and recovery using `restorecon`

---

## 📂 Repository Structure

```bash
iam-labs/
│── README.md
│── screenshots/
│   ├── lab1/
│   ├── lab2/
│   ├── lab3/
│   └── ...
│── commands/
│   ├── lab1.txt
│   ├── lab2.txt
│   └── ...
```

---

## 📸 Screenshots

Screenshots of each lab execution are included in the `screenshots/` folder as proof of practical work.

---

## ⚙️ Tools & Technologies

* Linux (Kali, Ubuntu, CentOS/AlmaLinux)
* Bash Shell
* Apache Web Server
* SELinux
* PAM (Pluggable Authentication Modules)
* ACL (Access Control Lists)

---

## 🎯 Key Learnings

* User and group management
* Role-based access control
* Password security policies
* File and directory permissions
* Advanced Linux security mechanisms (ACL, SELinux, PAM)

---

## 🔗 Submission Note

This repository serves as proof of practical implementation for the IAM labs.
All commands, configurations, and screenshots reflect the work completed during the course.

---

## 🚀 Author

**Shenyuy Goodness-Divine Tata**
nux labs for Identity and Access Management (IAM), covering user management, access control, authentication, and system security
