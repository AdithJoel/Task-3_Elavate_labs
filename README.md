# Task-3_Elavate_labs
# Basic Vulnerability Scan

This project is part of my cyber security internship task.  
I used Nessus Essentials to scan my own computer and check for common problems.

## What I Did
1. Installed Nessus Essentials.
2. Scanned my local computer (192.168.0.181).
3. Waited for the scan to finish.
4. Looked at all the issues found.
5. Wrote a short report and saved my results.

## Tools Used
- Nessus Essentials (free version)
- Windows 11 (scan target)

## Main Findings
The scan found a few medium level issues:

### 1. SMB Signing Not Required
SMB signing was not turned on.  
This means SMB traffic is not fully protected.

### 2. SSL Certificate Cannot Be Trusted
Some services use certificates that cannot be fully trusted.

### 3. SSL Self-Signed Certificate
A service used a certificate it made by itself.

### 4. SSL Certificate With Wrong Hostname
The certificate name did not match the computer name.

### 5. SSL Certificate Signed By Unknown Authority
One certificate was signed by a source that is not trusted.

## Fixes
- Turn on SMB signing.
- Use proper SSL certificates.
- Make sure certificate names match the system.
- Avoid self-signed certificates when possible.

## Files in This Repo
- **README.md** – explanation of the task  
- **report.pdf** – short written report  
- **screenshots/** – images from the scan 
