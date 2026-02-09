# week-2-port-scanning
Week 2 cybersecurity task -- Port scanning and analysis using Nmap on a local system.

Tool Used:
Nmap

Target System:
Local machine (192.168.1.10)

Objective:
The objective of this task was to perform a port scan on a local system to identify open ports and analyze the services running on those ports. This helps understand potential security exposure and attack surfaces.

Procedure:

1. Installed Nmap network scanning tool.
2. Identified the local IP address using the ipconfig command.
3. Performed a basic TCP scan using:
   nmap 192.168.1.10
4. Performed an advanced scan using:
   nmap -sS -sV 192.168.1.10
5. Recorded and analyzed the scan results.

Findings:
The scan revealed the following open ports and services:

* Port 135 (MSRPC): Used for Windows internal communication.
* Port 139 (NetBIOS): Enables file and printer sharing over the network.
* Port 445 (Microsoft-DS/SMB): Used for Windows file sharing.
* Port 5357 (WSDAPI): Supports device discovery on the network.
* Port 16992 (Intel AMT): Used for remote management functions.

Security Analysis:
Open ports indicate active services that could become potential attack points if misconfigured or left unpatched. While these services are normal for a Windows environment, limiting exposure and applying firewall rules can reduce risk.

Conclusion:
Port scanning is an essential cybersecurity technique for identifying exposed services. This task demonstrated how to use Nmap to evaluate system exposure and reinforced the importance of monitoring open ports to maintain system security.

