#  Wireshark Network Traffic Analysis

##  Task Overview
This project was completed as part of my Cyber Security Internship (Task 5).  
The goal was to **capture live network traffic using Wireshark**, filter it by protocol, and analyze the packet details.

---

##  Tools Used
- **Wireshark** – For capturing and analyzing network packets.
- **Web Browser / Ping Command** – To generate network traffic.

---

##  Repository Contents
- `network_capture.pcap` → Captured network traffic file.
- `screenshots/` → Protocol filter views from Wireshark.
- `README.md` → Documentation and analysis.

---

##  Steps Performed
1. Opened Wireshark and selected the active network interface.
2. Started packet capture and generated traffic by:
   - Visiting multiple websites.
   - Using the `ping` command for ICMP traffic.
3. Stopped the capture after ~2 minutes.
4. Used **display filters** to isolate specific protocols:
   - `arp`
   - `dns`
   - `http`
   - `icmp`
   - `tcp`
5. Saved the capture as a `.pcap` file and documented the findings.

---

##  Protocol Analysis

###  ARP (Address Resolution Protocol)
**Filter Used:** `arp`  
**Description:** ARP is used to map IP addresses to MAC addresses within a local network.  
**Observation:**  
- Requests like "Who has 10.0.2.2? Tell 10.0.2.15" indicate a device querying the MAC address of another device on the network.

**Screenshot:**  
![arp](https://github.com/user-attachments/assets/08598264-d5ed-4c79-a288-7b011911202d)

---

###  DNS (Domain Name System)
**Filter Used:** `dns`  
**Description:** DNS resolves human-readable domain names (e.g., google.com) to IP addresses.  
**Observation:**  
- Queries for domains like `google.com`, `youtube.com`, and `mozilla.net`.
- Both IPv4 (A) and IPv6 (AAAA) responses observed.

**Screenshot:**  
![dns](https://github.com/user-attachments/assets/a46b254a-6915-4f83-8d97-2352e43ed1b9)

---

###  HTTP (Hypertext Transfer Protocol)
**Filter Used:** `http`  
**Description:** HTTP is used to transfer web pages and resources between browsers and servers.  
**Observation:**  
- Requests like `GET /success.txt?ipv4` show the browser retrieving a text file.
- Responses contain status codes like `200 OK` indicating successful retrieval.

**Screenshot:**  
![http](https://github.com/user-attachments/assets/23200a2f-3ded-4a85-951b-44011caaf5fd)

---

###  ICMP (Internet Control Message Protocol)
**Filter Used:** `icmp`  
**Description:** ICMP is mainly used for diagnostic purposes like the `ping` command.  
**Observation:**  
- Echo requests and replies between my system and external IPs.
- TTL values and sequence numbers confirm successful round-trip communication.

**Screenshot:**  
![icmp](https://github.com/user-attachments/assets/f426a712-5396-4df9-8e9b-ab72e94d38bf)

---

###  TCP (Transmission Control Protocol)
**Filter Used:** `tcp`  
**Description:** TCP ensures reliable data transmission between devices.  
**Observation:**  
- TCP three-way handshakes (`SYN`, `SYN-ACK`, `ACK`) before HTTP communication.
- Packets carrying application data after connection establishment.

**Screenshot:**  
![tcp](https://github.com/user-attachments/assets/5605efd7-0aa1-4b1f-8fec-5833a1a98d39)

---

##  How to Open `.pcapng` File
1. Download and install **Wireshark** from [https://www.wireshark.org/](https://www.wireshark.org/).
2. Open the `.pcapng` file to view the captured packets and apply filters.

---

## 🎯 Outcome
- Captured and analyzed multiple network protocols.
- Learned to apply Wireshark display filters to isolate traffic types.
- Understood packet details for ARP, DNS, HTTP, ICMP, and TCP.

---
