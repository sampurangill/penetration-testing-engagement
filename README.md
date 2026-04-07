# Internal Network Penetration Test

## Overview
Conducted a full internal network penetration test as part of a simulated security engagement. The objective was to identify vulnerabilities, exploit weaknesses, and provide remediation strategies to improve the organization's security posture.

## Scope
- Internal network penetration testing
- Multiple target systems within a controlled lab environment
- Excluded: Denial of Service (DoS), Social Engineering

## Methodology
Followed a structured penetration testing methodology:

1. **Reconnaissance & Scanning**
   - Identified open ports and services using Nmap

2. **Enumeration**
   - Discovered vulnerable services and system configurations

3. **Exploitation**
   - Leveraged known vulnerabilities using Metasploit
   - Gained initial access to multiple systems

4. **Privilege Escalation**
   - Escalated access to SYSTEM/Administrator level
   - Used local exploit techniques

5. **Post-Exploitation**
   - Navigated file systems and accessed sensitive data
   - Identified lateral movement opportunities

6. **Reporting**
   - Documented vulnerabilities, impact, and remediation steps

## Tools Used
- Kali Linux
- Metasploit Framework
- Nmap

## Key Findings
- Exploited SMB vulnerabilities (EternalBlue, ms08-067) to gain remote access
- Identified multiple Remote Code Execution (RCE) vulnerabilities
- Successfully performed privilege escalation on several systems
- Discovered outdated and unpatched systems across the network
- Weak access controls allowed unauthorized data access

## Vulnerability Summary
- Critical: 2
- High: 6

## Example Attacks
- SMB Exploitation (EternalBlue - MS17-010)
- NetAPI Exploit (MS08-067)
- IIS WebDAV Exploitation
- Rejetto HFS Remote Command Execution
- Multiple privilege escalation exploits (Windows Kernel & Services)

## Impact
- Full system compromise achieved on multiple machines
- Unauthorized access to sensitive files and administrator accounts
- Demonstrated risk of lateral movement within the network

## Recommendations
- Apply regular system patching and updates
- Disable outdated protocols (e.g., SMBv1)
- Implement network segmentation
- Strengthen firewall configurations
- Enforce least privilege access controls
- Monitor and log suspicious activity

## Skills Demonstrated
- Network Scanning & Enumeration
- Vulnerability Exploitation
- Privilege Escalation
- Post-Exploitation Techniques
- Security Assessment & Reporting
