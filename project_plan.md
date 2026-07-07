# Web Application Penetration Testing on DVWA
## Project Plan

---

# Project Information

**Project Title:** Web Application Penetration Testing on DVWA

**Internship:** ApexPlanet Cybersecurity & Ethical Hacking Internship

**Task:** Task 5 – Capstone Project & Incident Response

**Project Type:** Web Application Security Assessment

**Platform:** Kali Linux

**Target Application:** Damn Vulnerable Web Application (DVWA)

**Prepared By:** Vadla Laxmi

**Date:** 7-Jul-2026

---

# Table of Contents

1. Introduction
2. Project Objective
3. Project Scope
4. Project Goals
5. Technologies Used
6. Tools Used
7. Lab Environment
8. Testing Methodology
9. Project Timeline
10. Expected Deliverables
11. Risk Assessment
12. Ethical Considerations
13. Expected Outcome
14. Conclusion

---

# 1. Introduction

Web applications are one of the most common targets for cyber attackers because they often contain vulnerabilities caused by insecure coding practices. Penetration testing is the process of evaluating the security of an application by safely simulating attacks in a controlled environment.

This project focuses on performing a complete penetration test on the Damn Vulnerable Web Application (DVWA). DVWA is intentionally designed with security flaws for educational purposes. The project demonstrates how common web vulnerabilities can be identified, exploited in a safe environment, analyzed, and mitigated using industry-standard security tools.

---

# 2. Project Objective

The primary objective of this project is to perform a comprehensive web application penetration test against DVWA using Kali Linux and identify security vulnerabilities in a controlled lab environment.

The project also aims to:

• Understand the penetration testing lifecycle.
• Perform reconnaissance and vulnerability assessment.
• Exploit common OWASP Top 10 vulnerabilities.
• Analyze attack evidence.
• Capture application logs.
• Simulate an incident response process.
• Recommend mitigation techniques.
• Prepare a professional penetration testing report.

---

# 3. Project Scope

This project is limited to the local DVWA application running inside a controlled virtual laboratory.

The assessment includes the following modules:

• SQL Injection
• Cross Site Scripting (Stored XSS)
• Cross Site Scripting (Reflected XSS)
• Command Injection
• File Inclusion
• Brute Force Authentication
• HTTP Request Analysis
• Web Server Enumeration
• Security Misconfiguration Identification

The following activities are NOT included:

• Testing external websites
• Cloud infrastructure testing
• Wireless attacks
• Social engineering attacks
• Denial of Service attacks
• Real-world exploitation

---

# 4. Project Goals

The project has the following goals:

• Build practical penetration testing skills.
• Learn web application attack techniques.
• Understand attacker methodology.
• Learn how vulnerabilities affect applications.
• Understand secure coding practices.
• Improve vulnerability reporting skills.
• Learn incident response procedures.
• Develop professional documentation.

---

# 5. Technologies Used

Operating System

• Kali Linux

Target Application

• DVWA (Damn Vulnerable Web Application)

Web Server

• Apache HTTP Server

Database

• MariaDB

Programming Languages

• PHP
• SQL

Browser

• Mozilla Firefox

---

# 6. Security Tools Used

## Nmap

Purpose:

• Host discovery
• Port scanning
• Service detection
• Operating system detection

---

## Nikto

Purpose:

• Web server vulnerability scanning
• Security misconfiguration detection
• Default file discovery

---

## Burp Suite

Purpose:

• Intercept HTTP requests
• Modify requests
• Analyze responses
• Manual security testing

---

## SQLMap

Purpose:

• Automated SQL Injection testing
• Database enumeration
• Table enumeration
• Data extraction

---

## Hydra

Purpose:

• Password auditing
• Brute force authentication testing

---

## Wireshark

Purpose:

• Packet capture
• HTTP traffic analysis
• Network troubleshooting

---

# 7. Lab Environment

Attacker Machine

Operating System:
Kali Linux

IP Address:
192.168.56.101

---

Target Machine

DVWA

Operating System:
Linux

Web Server:
Apache 2.4

Database:
MariaDB

IP Address:
192.168.56.102

---

Network Configuration

Host Only Adapter

The attacker machine and target machine communicate only inside the isolated virtual lab environment.

This ensures:

• Safe testing
• No Internet exposure
• Controlled environment

---

# 8. Penetration Testing Methodology

The project follows the standard penetration testing lifecycle.

## Phase 1 – Reconnaissance

Objectives

• Identify target IP
• Verify connectivity
• Gather initial information

Tools

• Ping
• Nmap

Expected Output

• Active host
• Open ports

---

## Phase 2 – Scanning

Objectives

• Discover services
• Identify versions
• Detect operating system

Tools

• Nmap
• Nikto

Expected Output

• Service list
• Web server information
• Security weaknesses

---

## Phase 3 – Enumeration

Objectives

• Discover application information
• Analyze HTTP requests
• Identify hidden functionality

Tools

• Burp Suite

Expected Output

• Cookies
• Parameters
• HTTP Requests

---

## Phase 4 – Exploitation

The following vulnerabilities will be tested.

### SQL Injection

Goal

Retrieve database information.

Tool

SQLMap

---

### Cross Site Scripting

Goal

Execute JavaScript within the browser.

Types

• Stored XSS
• Reflected XSS

---

### File Inclusion

Goal

Read sensitive server files.

---

### Command Injection

Goal

Execute operating system commands.

---

### Brute Force

Goal

Test password strength.

Tool

Hydra

---

## Phase 5 – Log Analysis

Objectives

Monitor

Apache Access Logs

Collect

Evidence

Analyze

Attack traces

---

## Phase 6 – Incident Response

Objectives

Detect

Contain

Eradicate

Recover

Document

the simulated security incident.

---

## Phase 7 – Reporting

Produce

Professional penetration testing report

Including

• Screenshots
• Commands
• Evidence
• Findings
• Recommendations

---

# 9. Project Timeline

| Phase | Activity |
|--------|----------|
| Phase 1 | Project Planning |
| Phase 2 | Reconnaissance |
| Phase 3 | Scanning |
| Phase 4 | Enumeration |
| Phase 5 | SQL Injection |
| Phase 6 | XSS Testing |
| Phase 7 | File Inclusion |
| Phase 8 | Command Injection |
| Phase 9 | Brute Force |
| Phase 10 | Log Analysis |
| Phase 11 | Incident Response |
| Phase 12 | Final Report |
| Phase 13 | GitHub Upload |
| Phase 14 | Presentation |

---

# 10. Expected Deliverables

The project will produce:

• Project Plan
• Network Diagram
• Nmap Scan Report
• Nikto Scan Report
• SQLMap Output
• Burp Suite Screenshots
• SQL Injection Screenshots
• XSS Screenshots
• File Inclusion Screenshots
• Command Injection Screenshots
• Hydra Output
• Apache Logs
• Incident Response Report
• Risk Assessment
• Mitigation Report
• Final Penetration Testing Report
• GitHub Repository
• Demonstration Video

---

# 11. Risk Assessment

The following risks are expected.

| Vulnerability | Severity |
|--------------|----------|
| SQL Injection | Critical |
| Command Injection | Critical |
| Stored XSS | High |
| File Inclusion | High |
| Reflected XSS | Medium |
| Brute Force | Medium |

---

# 12. Ethical Considerations

This penetration test is performed only against DVWA running inside a private laboratory.

No third-party systems are targeted.

No unauthorized access is attempted.

All testing follows responsible and ethical hacking principles.

---

# 13. Expected Outcome

Upon successful completion of this project, the following outcomes are expected:

• Identification of web application vulnerabilities.
• Practical understanding of penetration testing.
• Professional documentation skills.
• Knowledge of attack techniques.
• Understanding of secure coding practices.
• Incident response experience.
• GitHub portfolio project.
• Internship task completion.

---

# 14. Conclusion

This project demonstrates the complete lifecycle of a professional web application penetration test using DVWA. The assessment includes reconnaissance, scanning, exploitation, reporting, and incident response. The project strengthens practical cybersecurity skills while emphasizing responsible disclosure, ethical testing, and secure software development practices.

---

# References

1. OWASP Top 10
https://owasp.org/www-project-top-ten/

2. DVWA Documentation
https://github.com/digininja/DVWA

3. Nmap Official Documentation
https://nmap.org

4. Burp Suite Documentation
https://portswigger.net/burp

5. SQLMap Documentation
https://sqlmap.org

6. Nikto Documentation
https://github.com/sullo/nikto

7. Hydra Documentation
https://github.com/vanhauser-thc/thc-hydra
