# nmap_scan_results.txt
# Basic Network Scan using Nmap

## Objective
Perform a network scan to identify open ports and services on a target machine.

## Tool Used
Nmap

## Target
192.168.115.1

## Scan Command
nmap -T4 -A -v 192.168.115.1

## Open Ports and Services

80/tcp - HTTP  
Used for web servers. The scan detected Apache HTTP server.

135/tcp - MSRPC  
Microsoft Remote Procedure Call service used by Windows.

139/tcp - NetBIOS-SSN  
Used for file and printer sharing on Windows networks.

443/tcp - HTTPS  
Secure web communication using SSL/TLS.

445/tcp - Microsoft-DS  
SMB service used for Windows file sharing.

903/tcp - VMware Authentication  
Used for VMware remote console authentication.

3306/tcp - MySQL  
Database service used by applications to store data.

## Conclusion
The scan successfully identified several open ports and running services on the target machine. Identifying open ports helps security professionals detect potential vulnerabilities and improve system security.
