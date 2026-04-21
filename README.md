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



Results
1. Sensitive directories discovered during enumeration

2. SQL Injection attempts blocked by WAF

3. Minor configuration issues identified by OWASP ZAP

4. Overall: Application resilient against common web attacks



Recommendations

1. Enable HTTPS encryption

2. Regularly update PrestaShop and modules

3. Restrict access to administrative directories

4. Implement strong password policies

5. Review firewall logs frequently

6. Disable unnecessary directories/services



 Contents Repository
  
   Documentation
- [Full Security Assessment Report (PDF)](./Docs/Web%20Application%20Security%20Assessment%20Report.pdf)


  Screenshots
- [Gobuster Scan Result](./Screenshot/Gobuster%20Scan%20Result.png)
- [SQLMap Results](./Screenshot/SQLMap%20Results.png)
- [WAF Blocking Attack 1](./Screenshot/WAF%20Blocking%20Attack%201.png)
- [WAF Blocking Attack 2](./Screenshot/WAF%20Blocking%20Attack%202.png)



  Skills Demonstrated
- Penetration testing methodology  
- Vulnerability scanning & enumeration  
- SQL Injection testing & mitigation  
- Web Application Firewall (WAF) configuration  
- Secure coding & defensive recommendations  




Conclusion

This project demonstrates hands-on experience in penetration testing, vulnerability scanning, and defensive security implementation.

It highlights the importance of proactive security measures in protecting modern e-commerce platforms. additional It reflects my ability

to conduct structured security assessments and implement effective defensive strategies.


 Key Takeaways
- Demonstrated ability to assess real‑world applications.  
- Balanced offensive and defensive security practices.  
- Produced professional documentation and recommendations.  


