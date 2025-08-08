#  Task 4 – Firewall Setup and Management (UFW)

**Cyber Security Internship**

##  Objective

The goal of this task was to understand and practice basic firewall management on a Linux system using UFW (Uncomplicated Firewall). The task involved configuring firewall rules to control network traffic by allowing or blocking specific ports.

---

##  What Was Done

- Enabled the UFW firewall on a Linux system.
- Viewed the existing firewall rules to understand current configurations.
- Added a rule to block port 23 (commonly used by Telnet) to enhance security.
- Tested the firewall by attempting to access the blocked port.
- Allowed SSH access (port 22) to ensure safe remote connectivity.
- Removed the block rule to return the system to its original state.

---

##  How a Firewall Filters Traffic

A firewall works as a security barrier between a trusted network and untrusted external sources. It monitors incoming and outgoing traffic and filters it based on a set of predefined rules.

- **Inbound rules** determine what external traffic is allowed into your system.
- **Outbound rules** control which data your system can send out.
- Firewalls can allow or block traffic based on port numbers, IP addresses, or protocols.
- Tools like UFW make it easier to manage these rules without needing deep technical knowledge.

By carefully configuring these rules, a firewall helps prevent unauthorized access, data breaches, and other network-based attacks.

---

##  Outcome

This task helped build a strong foundation in firewall configuration and gave practical knowledge of how to secure a Linux system by managing allowed and blocked network traffic.

