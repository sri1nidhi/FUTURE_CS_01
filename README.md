# FUTURE_CS_01
Vulnerability Assessment Report of demo.testfire.net using Nmap, OWASP ZAP (passive scan), and Browser DevTools. Includes identified risks, screenshots, and remediation steps.


# Vulnerability Assessment Report

##  Project Overview
This project presents a vulnerability assessment of a live web application:
http://demo.testfire.net

The assessment was conducted using ethical, read-only techniques to identify common security weaknesses without exploiting the system.

---

##  Objective
- Analyze a public website for security vulnerabilities
- Classify risks (Low / Medium / High)
- Explain issues in simple language
- Suggest practical remediation steps

---

##  Tools Used
- Nmap (Port & Service Analysis)
- OWASP ZAP (Passive Vulnerability Scanning)
- Browser Developer Tools (Headers & Cookies Analysis)
- Kali Linux (Virtual Machine)

---

##  Methodology
1. Performed port scanning using Nmap
2. Conducted passive vulnerability scanning using OWASP ZAP
3. Analyzed HTTP headers and cookies using browser DevTools
4. Collected and documented findings with screenshots

---

##  Key Findings

###  High Risk
- Missing CSRF Protection
- Insecure Cookies (Missing SameSite / Secure attributes)

###  Medium Risk
- Missing Security Headers (CSP, X-Frame-Options, X-Content-Type-Options)
- Information Disclosure (Server details exposed)
- No HTTPS Enforcement

###  Low Risk
- Open ports exposure

---

##  Recommendations
- Implement security headers (CSP, HSTS, X-Frame-Options)
- Secure cookies with HttpOnly, Secure, and SameSite flags
- Enable HTTPS across the application
- Hide server and technology details
- Implement CSRF protection mechanisms

---

## Evidence
All findings are supported with screenshots:
- Nmap scan results
- OWASP ZAP alerts
- Browser DevTools (headers & cookies)

---

##  Scope & Ethics
- Only public-facing pages were tested
- No exploitation or harmful activity was performed
- Passive scanning techniques only

---

##  Conclusion
The application contains several medium to high-risk vulnerabilities. Addressing these issues will significantly improve its overall security posture.

---

##  Author
Nadiminte Srinidhi Reddy
