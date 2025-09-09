# firewall
###### *DISCLAIMER: The following code is only for Ubuntu.*

### Features
1) Block IP addresses
2) Block access to certain ports 
3) Block specifed prefixes of IP address (to block networks)
4) Block too many requests made by the same IP in a short period of time (user can specify threshold and time)

### Steps to Run
1) Type the following terminal command: 
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;iptables -I INPUT -d 192.168.0.0/24 -j NFQUEUE --queue-num 1
2) Fill out the rules in the JSON file as follows:
<img width="407" height="144" alt="config" src="https://github.com/user-attachments/assets/ae70566a-5365-4730-bece-127da2688ff4" />

3) Execute firewall.py using python3

### Requirements
1) netfilterqueue
2) scapy
