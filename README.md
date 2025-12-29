Web Application Penetration Testing (DVWA)
📌 Project Overview

This project demonstrates Web Application Penetration Testing using DVWA (Damn Vulnerable Web Application).
The objective is to identify, exploit, and document common web vulnerabilities in a controlled environment and understand mitigation strategies.

🎯 Objectives

Identify common web vulnerabilities

Perform controlled exploitation

Understand attack techniques

Apply mitigation strategies

Document findings professionally

🛠️ Tools & Technologies
Tool	Purpose
Kali Linux	Penetration testing OS
DVWA	Vulnerable web application
Apache	Web server
MariaDB	Database
Burp Suite	Intercepting & modifying HTTP requests
Browser	Testing and exploitation
🧱 Project Architecture
Attacker (Kali Linux)
        |
        | HTTP Requests
        v
DVWA Web Application
        |
        v
     MariaDB

🔍 Vulnerabilities Tested
1️⃣ SQL Injection

Extracted database details using UNION-based queries

Retrieved usernames and password hashes

Example Payload:

' UNION SELECT user(), database() #

2️⃣ Cross-Site Scripting (XSS)
Reflected XSS:
<script>alert('XSS')</script>

Stored XSS:
<script>alert('XSS')</script>

3️⃣ Command Injection
127.0.0.1; whoami


Allowed execution of system commands.

4️⃣ Brute Force Attack

Used Burp Suite Intruder

Password list: rockyou.txt

Successfully bypassed authentication

🚨 Incident Response
Identification

Detected unauthorized login attempts.

Containment

Blocked attacker IP using firewall

Disabled compromised accounts

Eradication

Restarted services

Removed malicious activity

Recovery

Reset credentials

Monitored system logs

🔐 Security Recommendations

Input validation & sanitization

Prepared SQL statements

Account lockout mechanisms

CAPTCHA & MFA

Regular security audits

📁 Project Structure
DVWA-Pentest/
│── README.md
│── Screenshots/
│   ├── SQL_Injection/
│   ├── XSS/
│   ├── Command_Injection/
│   ├── BruteForce/
│── Report/
│   └── Final_Report.pdf

📘 Learning Outcomes

Hands-on experience in ethical hacking

Understanding of OWASP Top 10 vulnerabilities

Practical incident response skills

Improved security awareness
