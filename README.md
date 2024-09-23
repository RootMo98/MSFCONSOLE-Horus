# MSFCONSOLE-Horus
Automated Metasploit Recon &amp; Enumeration
This project focuses on creating an advanced reconnaissance and vulnerability scanning script for Metasploit, designed to automate and streamline the process of target discovery, service enumeration, and vulnerability identification. The script ensures efficient scanning by:

Checking for open ports first before running specific service vulnerability scans.
Running targeted Nmap scripts only for services that are confirmed to be active on the target, minimizing unnecessary scanning and optimizing performance.
Saving detailed scan results in a structured format for easy review and analysis.
Current Features:

Full Port Scan: Aggressively scans all open ports on the target machine.
OS Detection and Service Versioning: Performs OS fingerprinting and service version detection to understand the target’s operating system and running services.
Conditional Vulnerability Scanning: Runs Nmap vulnerability scripts only if specific services are detected (e.g., SMB, HTTP, WinRM), improving scan efficiency.
SMB vulnerability scan: Only runs if port 445 is open.
HTTP vulnerability scan: Runs on open ports 80 and 443.
WinRM enumeration: Only runs if port 5985 is open.
Structured Reporting: Saves and consolidates results into a detailed report file for each target, making it easy to analyze the findings.
Planned Enhancements:

Add support for more services and ports, such as FTP (port 21), MySQL (port 3306), and more.
Integrate additional Nmap scripts for comprehensive vulnerability scanning across a wider range of protocols.
Automate integration with tools like Searchsploit and Eyewitness for exploit suggestions and visual analysis of discovered web services.
Support DNS enumeration, UDP scanning, and other advanced techniques for deeper recon on internal networks.
Auto-save scan results to different formats (e.g., HTML reports for easier review).
