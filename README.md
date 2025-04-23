# OPS310-LDAP-Email-Server
Full-stack email system using Postfix, Dovecot, and LDAP for centralized authentication. IMAP/SMTP integration with end-to-end testing. Completed for OPS310 at Seneca Polytechnic.
# LDAP-Integrated Email Server Deployment – OPS310 Lab 5 & Assignment 2

**Course:** OPS310 – Cloud Platform Management  
**Date:** April 2025  
**Institution:** Seneca Polytechnic

---

## 🧠 Overview
This project simulated the deployment of a secure, LDAP-authenticated email system using three core services: Postfix (SMTP), Dovecot (IMAP), and OpenLDAP (authentication). All systems were configured on separate Linux VMs and integrated to provide centralized login and full email functionality.

---

## 🔧 System Architecture

| VM          | Service     |
|-------------|-------------|
| `authsrv`   | OpenLDAP (Directory Server)  
| `mailsrv`   | Postfix (SMTP), Dovecot (IMAP)  
| `client`    | Thunderbird + Command-line email tools for testing  

---

## 🔐 Configuration Highlights

- **LDAP Server:**  
  - Created users, groups, and custom OU structure  
  - Configured for remote authentication

- **Postfix (SMTP):**  
  - LDAP user authentication for sending mail  
  - TLS encryption enabled

- **Dovecot (IMAP):**  
  - LDAP integration via `dovecot-ldap.conf`  
  - Secure login and retrieval of messages via Thunderbird and CLI

---

## 🧪 Testing & Validation

- Sent test messages via `swaks` and Thunderbird  
- Verified LDAP login via `/var/log/mail.log` and live sessions  
- Confirmed mail flow from sender to recipient and inbox delivery  
- Screenshots and logs captured for SMTP and IMAP validation

---

## 📎 Documentation

This project was submitted as a full lab report, including:
- Configuration steps  
- User/Group structure  
- Email send/receive flow  
- Screenshots of successful login and mail retrieval  

(*Report not included in repo upload.*)

---

## 🧠 Skills Demonstrated
- Postfix (SMTP server configuration)  
- Dovecot (IMAP integration)  
- LDAP (centralized user auth)  
- Linux-based email systems  
- Secure mail delivery and testing

---

## ✅ Project Status
- ✔️ All services integrated and tested  
- ✔️ LDAP user authentication working for mail services  
- ✔️ Email successfully sent and retrieved
