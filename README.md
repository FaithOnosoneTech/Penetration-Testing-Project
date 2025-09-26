## Penetration-Testing-Project. _Operation Breach and Patch!_
This Repository is a project  to determine the security strength of TecNova Ltd Networks and Systems.

### The Project is to simulate internal penetration test on TechNova Ltd using their Kali Linux machine in order to identify vulnerabilities on a simulated network, successfully exploit and identify critical weaknesses in their network and provide a professional report with findings and Recommendations.

### Executive Summary (High Overview)
(see Screenshots 1ai)

### The Project Tools
(see Screenshots 2ai)

### PHASE1: Reconnaissance steps and findings
Use nmap to:
  - Discover live hosts in the network. (see Screenshots 3ai)
  - Perform service and version detection on open ports. (see Screenshots 3aii)

Use Netcat (or Telnet) to: 
  - Grab service banners and identify versions of exposed services. (see Screenshots 3bi)

### Phase2: Vulnerability Scanning
  - Using Nessus Essentials to scan for vulnerabilities on the discovered systems (see Screenshots 4ai, 4aii, 4bi & 4bii)
  - Documenting and prioritizing the vulnerabilities based on severity and potential impact.

    Note:  only on 4 major vulnerabilities which were further exploited in Phase3 of the Project.
      -  VNC no-authentication on port 5900.
      -  SMTP misconfiguration on port 25. 
      -  MS17-010 (CVE-2017-0144) on Windows SMB Port 445.
      -  RPC exposure on port 135.
     
### Phase 3: Exploitation
Four critical vulnerabilities identified in the Nessus scan will be exploited using Metasploit to gain Access to the Systems:
 
  #### Metasploitable2 (IP- 192.168.56.5):
      -  Setting up Msfconsole and Workplace (see Screenshots 5ai)
      -  VNC no-authentication on port 5900- Full Desktop Control (see Screenshots 5bi, 5bii, 5biii & 5biv)
      -  SMTP misconfiguration on port 25- Command Execution (see Screenshots 5ci, 5cii & 5ciii)

  #### Windows10 (IP- 192.168.56.11):
      -  Generating and Transfering Payload for Port135 to Target System (see Screenshots 5di, 5dii & 5diii)
      -  Setting up Msfconsole and Workplace (see Screenshots 5ei)
      -  RPC Exposure on Port 135- System Shell (see Screenshots 5fi, 5fii & 5fiii)
       -  Generating and Transfering Payload for Port445 to Target System (see Screenshots 5gi, 5gii & 5giii)
      -  EternalBlue SMB exploit on Port 445→ Remote Code Execution (see Screenshots 5hi, 5hii & 5hiii).


