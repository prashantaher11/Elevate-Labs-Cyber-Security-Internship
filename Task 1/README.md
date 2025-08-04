# 🔍 Task 1: Nmap Scan Report

## 📄 Overview

This task involved scanning the local network `192.168.56.101/24` using `nmap` to identify live hosts and open ports, followed by a basic security risk assessment based on the scan results.

---

## 1️⃣ IP Addresses and Open Ports Found

| **IP Address**     | **Open Ports**                                      | **Service Name**                                |
|--------------------|-----------------------------------------------------|--------------------------------------------------|
| `192.168.56.1`     | 135/tcp, 139/tcp, 445/tcp, 902/tcp, 912/tcp, 3306/tcp | MSRPC, NetBIOS-SSN, Microsoft-DS, ISS RealSecure, Apex Mesh, MySQL |
| `192.168.56.100`   | None (All ports filtered)                           | —                                                |
| `192.168.56.101`   | None (All ports closed)                             | —                                                |

---

## 2️⃣ Potential Security Risks from Open Ports

| **Port** | **Service**       | **Potential Security Risk**                                                                 |
|----------|------------------|---------------------------------------------------------------------------------------------|
| 135/tcp  | MSRPC            | Susceptible to DCOM attacks; known target of malware like WannaCry.                         |
| 139/tcp  | NetBIOS-SSN      | Can be exploited for SMB relay attacks and information disclosure.                          |
| 445/tcp  | Microsoft-DS     | Vulnerable to EternalBlue, ransomware attacks; commonly abused in SMB vulnerabilities.      |
| 902/tcp  | ISS RealSecure   | Often VMware-related; may allow unauthorized VM control if unsecured.                       |
| 912/tcp  | Apex Mesh        | Uncommon; may represent custom or misconfigured services, often lacking authentication.     |
| 3306/tcp | MySQL            | Can lead to full DB compromise if weak credentials or open access from untrusted networks.  |

---

## 🛠️ Tools Used

- **Command Used:**  
  ```bash
  nmap -sS 192.168.56.101/24

