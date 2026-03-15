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

Documented Findings
Open Ports and Their Significance
Port 80 (HTTP)
Service: Web Server (Apache HTTPD)
Significance:
Port 80 is used for HTTP web traffic. It allows users to access websites hosted on the server. If not properly secured, attackers may exploit web vulnerabilities.
Port 135 (MSRPC)
Service: Microsoft Remote Procedure Call
Significance:
This port allows Windows systems to communicate with other services and applications on a network. Attackers sometimes target it to exploit Windows vulnerabilities.
Port 139 (NetBIOS-SSN)
Service: NetBIOS Session Service
Significance:
Used for file and printer sharing in Windows networks. If exposed to the internet, it may allow unauthorized access to shared files.
Port 443 (HTTPS)
Service: Secure Web Server
Significance:
Port 443 is used for secure web communication using SSL/TLS encryption. It protects data exchanged between the user and the website.
Port 445 (Microsoft-DS / SMB)
Service: SMB File Sharing
Significance:
This port is used for Windows file sharing and network resources. Many cyberattacks target SMB vulnerabilities if the system is not patched.
Port 903 (VMware Authentication)
Service: VMware Authentication Service
Significance:
This port is used by VMware remote console services for authentication and communication with virtual machines.
Port 3306 (MySQL Database)
Service: MySQL / MariaDB Database
Significance:
Port 3306 is used by database servers to store and manage application data. If exposed publicly without proper authentication, it can lead to data breaches.

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
