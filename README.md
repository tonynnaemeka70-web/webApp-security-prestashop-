 PrestaShop Web Application Security Assessment

 Project Overview
 
This repository documents a security assessment performed on a deployed PrestaShop web application.

The project demonstrates attack and defense security validation, showcasing practical penetration testing techniques and defensive

implementations using a Web Application Firewall (WAF).

- Assessment Type: Attack & Defense Security Validation  
- Author: Nweke Nnaemeka Anthony  
- Role: Cybersecurity Intern  
- Date: March 13, 2026  



 Objectives
- Identify potential vulnerabilities in the web application  
- Simulate real-world attack techniques  
- Implement defensive security mechanisms  
- Validate the effectiveness of deployed protection systems  



 Tools & Technologies
- sqlmap SQL injection testing  
- Gobuster Directory enumeration  
- OWASP ZAP Automated vulnerability scanning  
- curl Manual request testing  
- ModSecurity Web Application Firewall  



 Attack Simulations
1. Directory Enumeration  
   - Discovered sensitive directories (`admin`, `modules`, `config`, `themes`).  

2. SQL Injection Testing 
   - No vulnerabilities detected.  
   - WAF successfully blocked malicious payloads.  

3. Automated Vulnerability Scanning (OWASP ZAP) 
   - Identified missing security headers, cookie misconfigurations, and minor information disclosure issues.  



 Defense Implementation
 
A Web Application Firewall (ModSecurity) was configured with custom rules to block:
- SQL Injection attempts  
- XSS attempts  
- Directory Traversal attempts  

Example Rule:
```bash
SecRule ARGS "@rx (?i:union.*select)" \
"id:11001,phase:2,deny,status:403,msg:'SQL Injection Attempt

Results
Sensitive directories discovered during enumeration

SQL Injection attempts blocked by WAF

Minor configuration issues identified by OWASP ZAP

Overall: Application resilient against common web attacks


Recommendations
Enable HTTPS encryption

Regularly update PrestaShop and modules

Restrict access to administrative directories

Implement strong password policies

Review firewall logs frequently

Disable unnecessary directories/services


Repository Contents
Report: Full PDF security assessment

Screenshots: Evidence of attack simulations and defenses

Config: Custom ModSecurity rules


Conclusion
This project demonstrates hands-on experience in penetration testing, vulnerability scanning, and defensive security implementation.

It highlights the importance of proactive security measures in protecting modern e-commerce platforms.

