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
![screenshot]()
### 🔹 Lab 1: Assigning Limited Sudo Privileges

This lab demonstrates how to create users and assign different levels of administrative (sudo) privileges using the /etc/sudoers file.

* Created three users(lionel, katelyn, and maggie) were created using the useradd command. Passwords were assigned using the passwd command to enable login.
![screenshot1](<img width="818" height="920" alt="Screenshot 2026-03-27 233120" src="https://github.com/user-attachments/assets/81562024-7515-4aaf-b1ec-3840cf662bff" />)

* Configured `/etc/sudoers` using `visudo`
   The STORAGE alias was enabled by uncommenting it.
   Specific privileges were assigned:
lionel: Full administrative privileges.
katelyn: Limited to checking SSH service status.
maggie: Granted permissions defined under the STORAGE alias.
  ![screenshot2](<img width="944" height="942" alt="Screenshot 2026-03-27 233636" src="https://github.com/user-attachments/assets/af7e114c-7e6f-4df2-90d6-fb702a5d5f1c" />)
  
* Implemented role-based access control(Testing users capabilites on the system)
Lionel
![screentshot3](<img width="870" height="953" alt="Screenshot 2026-03-27 234357" src="https://github.com/user-attachments/assets/18451d84-8fda-4426-aa6c-cad1c883a84b" />)
Katelyn
![screenshot4](<img width="662" height="661" alt="Screenshot 2026-03-27 234856" src="https://github.com/user-attachments/assets/f2889e05-bfdf-42e6-adb9-0d35a88e77cb" />)
Maggie
![screenshot5](<img width="709" height="694" alt="Screenshot 2026-03-27 235913" src="https://github.com/user-attachments/assets/8c0efc89-a410-4e18-be72-11f1316a5bb0" />)

---

### 🔹 Lab 2: Disabling the Sudo Timer

This lab demonstrates how to control sudo session timeout behavior.
After entering the password once, multiple sudo commands were executed without re-authentication.

![screenshot6](<img width="682" height="631" alt="Screenshot 2026-03-28 000743" src="https://github.com/user-attachments/assets/e4a11d12-89db-413b-81d5-fcb7631b85db" />)

* Used `sudo -k` to reset authentication. The system required the password again which confirms timer reset.

![screenshot7](<img width="597" height="598" alt="Screenshot 2026-03-28 000927" src="https://github.com/user-attachments/assets/bcea5349-e6a8-4b9f-a554-5d67c358a27c" />
)
* Configured `timestamp_timeout` in sudoers
* Applied user-specific timeout policies `Defaults:lionel timestamp_timeout = 0` Only lionel is affected; other users retained default behavior.

![screenshot8](<img width="706" height="96" alt="image" src="https://github.com/user-attachments/assets/f08f2bd5-034a-4362-ad9d-2622d37e1fcc" />
)  

![screenshot9](<img width="707" height="578" alt="image" src="https://github.com/user-attachments/assets/572fc6df-161f-45c4-b2d6-7ea65a187658" />
)

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
