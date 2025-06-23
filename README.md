# Tools Used
Nmap: A free and open-source network scanner used for network discovery and security auditing.
1. Identifying Local IP Range
Before performing the scan, the local IP address and subnet mask were identified using the `ipconfig` command in the Windows Command Prompt.
My IP Address: 192.168.139.141
Default Gateway: 192.168.1.1
Subnet Mask: 255.255.255.0
Based on this, the local IP range for scanning was determined to be `192.168.1.0/24`.

2. Performing TCP SYN Scans with Nmap
#Scan 1: Single Host Scan
nmap -sS 192.168.235.141
Results:
The scan of `192.168.235.141` showed the following open ports:
135/tcp: msrpc
139/tcp: netbios-ssn
445/tcp: microsoft-ds
2869/tcp: icslap
3306/tcp: mysql
3389/tcp: ms-wbt-server
5357/tcp: wsdapi
