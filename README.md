# 🛡️ Web Application Penetration Testing on DVWA

![Platform](https://img.shields.io/badge/Platform-Kali%20Linux-blue)
![Application](https://img.shields.io/badge/Target-DVWA-red)
![Language](https://img.shields.io/badge/Language-PHP%20%7C%20SQL-green)
![Status](https://img.shields.io/badge/Project-Completed-success)
![License](https://img.shields.io/badge/License-Educational-yellow)

---

# 📖 Project Overview

This project was completed as part of the **ApexPlanet Cybersecurity & Ethical Hacking Internship (Task 5 – Capstone Project & Incident Response).**

The objective of this project is to perform a complete **Web Application Penetration Test** on the **Damn Vulnerable Web Application (DVWA)** using **Kali Linux** in a controlled laboratory environment.

The project demonstrates the complete penetration testing lifecycle including:

- Reconnaissance
- Scanning
- Enumeration
- Vulnerability Assessment
- Exploitation
- Log Analysis
- Incident Response
- Reporting
- Mitigation Recommendations

> **Disclaimer**
>
> This project was performed **only on DVWA running in a local virtual lab** for educational purposes. No unauthorized systems were targeted.

---

# 🎯 Objectives

The primary objectives of this project are:

- Understand Web Application Penetration Testing
- Perform vulnerability assessment on DVWA
- Identify OWASP Top 10 vulnerabilities
- Demonstrate exploitation techniques
- Capture attack evidence
- Analyze Apache server logs
- Simulate Incident Response
- Recommend mitigation strategies
- Prepare a professional penetration testing report

---

# 🖥️ Lab Environment

## Attacker Machine

| Item | Value |
|------|------|
| Operating System | Kali Linux |
| IP Address | 192.168.56.101 |

---

## Target Machine

| Item | Value |
|------|------|
| Application | DVWA |
| Web Server | Apache 2.4 |
| Database | MariaDB |
| IP Address | 192.168.56.102 |

---

## Network Type

Host-Only Network

The attacker and target communicate only within the virtual laboratory.

---

# 🛠️ Tools Used

| Tool | Purpose |
|------|----------|
| Kali Linux | Attacker Machine |
| DVWA | Vulnerable Web Application |
| Nmap | Port Scanning |
| Nikto | Web Server Scanning |
| Burp Suite | HTTP Request Interception |
| SQLMap | SQL Injection Automation |
| Hydra | Password Auditing |
| Wireshark | Packet Analysis |
| Apache | Web Server |
| MariaDB | Database |

---

# 📂 Project Structure

```
Task5-DVWA-Penetration-Testing/

│

├── README.md

├── project_plan.md

├── network_diagram.png

│

├── reports/

│ ├── nmap.txt

│ ├── nikto.txt

│ ├── final_report.pdf

│

├── screenshots/

│ ├── 01_lab_setup.png

│ ├── 02_ping.png

│ ├── 03_nmap.png

│ ├── 04_nikto.png

│ ├── 05_burpsuite.png

│ ├── 06_sql_injection.png

│ ├── 07_sqlmap.png

│ ├── 08_xss.png

│ ├── 09_file_inclusion.png

│ ├── 10_command_injection.png

│ ├── 11_hydra.png

│ ├── 12_logs.png

│

├── logs/

│ └── access.log

│

├── incident_response/

│ └── report.md

│

└── scripts/

```

---

# 🔬 Penetration Testing Methodology

The project follows the standard penetration testing lifecycle.

## Phase 1 – Project Planning

- Define project objectives
- Define project scope
- Identify tools
- Prepare lab environment

---

## Phase 2 – Reconnaissance

Performed:

- IP Discovery
- Ping Test
- Host Verification

Commands Used

```bash
ip a

ping 192.168.56.102
```

---

## Phase 3 – Network Scanning

Performed:

- Basic Scan
- Version Detection
- OS Detection
- Aggressive Scan

Commands

```bash
nmap 192.168.56.102

nmap -sV 192.168.56.102

sudo nmap -O 192.168.56.102

nmap -A 192.168.56.102
```

---

## Phase 4 – Web Server Scanning

Nikto was used to detect

- Security Misconfiguration
- Default Files
- Missing Headers
- Vulnerable Services

Command

```bash
nikto -h http://192.168.56.102
```

---

## Phase 5 – Burp Suite

Burp Suite was used to

- Capture Requests
- Analyze Cookies
- Modify HTTP Requests
- Inspect Responses

---

## Phase 6 – SQL Injection

Objective

Identify SQL Injection vulnerability.

Tools

- Manual Testing
- SQLMap

Activities

- Manual SQL Injection
- Database Enumeration
- Table Enumeration
- Data Extraction

---

## Phase 7 – Cross Site Scripting

Performed

- Stored XSS
- Reflected XSS

Payload Example

```html
<script>alert('Task5')</script>
```

---

## Phase 8 – File Inclusion

Payload

```
../../../../etc/passwd
```

Purpose

Read sensitive server files.

---

## Phase 9 – Command Injection

Payload

```
127.0.0.1; whoami
```

Purpose

Execute Linux commands.

---

## Phase 10 – Brute Force

Tool

Hydra

Purpose

Password Auditing

---

## Phase 11 – Log Analysis

Apache Access Logs were monitored using

```bash
sudo tail -f /var/log/apache2/access.log
```

---

## Phase 12 – Incident Response

Incident Response Process

- Detection
- Containment
- Eradication
- Recovery
- Lessons Learned

---

# 🚨 Vulnerabilities Tested

| Vulnerability | Severity |
|--------------|----------|
| SQL Injection | Critical |
| Command Injection | Critical |
| File Inclusion | High |
| Stored XSS | High |
| Reflected XSS | Medium |
| Brute Force | Medium |

---

# 🛡️ Mitigation Techniques

### SQL Injection

- Prepared Statements
- Parameterized Queries
- Input Validation

---

### Cross Site Scripting

- Input Validation
- Output Encoding
- Content Security Policy

---

### File Inclusion

- Restrict File Paths
- Validate User Input
- Disable Remote Inclusion

---

### Command Injection

- Whitelist Commands
- Input Sanitization
- Avoid Shell Execution

---

### Brute Force

- Account Lockout
- Strong Password Policy
- Multi-Factor Authentication

---

# 📊 Project Outcomes

Successfully Completed

- Project Planning
- Reconnaissance
- Nmap Scan
- Nikto Scan
- Burp Suite Analysis
- SQL Injection Testing
- XSS Testing
- File Inclusion Testing
- Command Injection Testing
- Brute Force Demonstration
- Log Analysis
- Incident Response Simulation
- Risk Assessment
- Professional Report
- GitHub Documentation

---

# 📚 Learning Outcomes

Through this project I gained practical experience in

- Web Application Security
- Penetration Testing
- Vulnerability Assessment
- Network Scanning
- Web Server Analysis
- SQL Injection
- Cross Site Scripting
- Incident Response
- Security Reporting
- Secure Coding Practices

---

# 📁 Deliverables

- Project Plan
- Network Diagram
- Nmap Report
- Nikto Report
- SQLMap Results
- Burp Suite Screenshots
- Vulnerability Screenshots
- Apache Logs
- Incident Response Report
- Risk Assessment
- Final Report
- GitHub Repository

---

# 📷 Sample Screenshots

The repository contains screenshots for

- Lab Setup
- Ping Test
- Nmap Scan
- Nikto Scan
- Burp Suite
- SQL Injection
- SQLMap
- XSS
- File Inclusion
- Command Injection
- Hydra
- Apache Logs

---

# 📖 References

- OWASP Top 10
- DVWA Documentation
- Nmap Documentation
- Burp Suite Documentation
- SQLMap Documentation
- Nikto Documentation
- Hydra Documentation

---

# 👨‍💻 Author

**Name:** Vadla Laxmi

**Internship:** ApexPlanet Cybersecurity & Ethical Hacking Internship

**Project:** Task 5 – Capstone Project & Incident Response

---

# ⭐ Acknowledgement

I would like to thank **ApexPlanet Software Pvt. Ltd.** for providing this internship opportunity and hands-on cybersecurity tasks that helped me gain practical experience in web application security, penetration testing, and incident response.

---

## ⚠️ Disclaimer

This project is intended **strictly for educational purposes**. All testing was conducted on **DVWA** within a private virtual laboratory. Do **not** use these techniques against systems you do not own or do not have explicit permission to test.
