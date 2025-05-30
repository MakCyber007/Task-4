# Task-4
# Firewall Configuration on Windows

## 📌 Task Overview  
This project involves configuring and testing firewall rules on **Windows Defender Firewall**
### **Objective**  
- Configure inbound and outbound firewall rules to block or allow network traffic.  
- Test the firewall rule for **Telnet (Port 23)**.  
- Document configuration steps, commands used, and rule explanations.

## 🔧 Tools Used  
- **Windows Defender Firewall** (GUI)  
- **PowerShell Commands**  
- **Nmap** (Network Scanning)  

## 📂 Deliverable Files  
This repository includes the following files:

1. **All_Firewall_Rules_through_PowerShell.txt**  
   - Extracted firewall rules using: `Get-NetFirewallRule > All_Firewall_Rules_through_PowerShell.txt`  

2. **Creating new firewall rule.pdf**  
   - Step-by-step documentation of rule creation using **Windows Defender Firewall (GUI)**.  

3. **PowerShell commands and Configuring Firewall rules.pdf**  
   - Screenshots of inbound and outbound firewall rules, PowerShell commands used.  
   - Documentation of additional rules created based on **Nmap scan findings**.  

4. **Testing the rule.pdf**  
   - Demonstrates the testing of **Telnet Port 23** rule by attempting a connection (`telnet localhost 23`).  

5. **README.md (This File!)**  
   - Overview of the task, tools, files, and security insights.  

## 🛡️ Firewall Rules Implemented  
The following firewall rules were created:

### **Inbound Rules**
- **Block Inbound Telnet (Port 23)** – Prevents remote Telnet access.  
- **Block Inbound MSRPC (Port 135)** – Blocks Microsoft Remote Procedure Calls.  
- **Block Inbound NetBIOS (Port 139)** – Disables legacy file-sharing requests.  
- **Block Inbound SMB (Port 445)** – Prevents unauthorized access and malware risks.  

### **Outbound Rules**
- **Block Outbound HTTP (Port 80)**  – Restricts unencrypted web requests for security.  

## 🔍 Testing Firewall Rules  
After implementing rules, I tested them using:  
- **Telnet Client** (`telnet localhost 23`) to check rule enforcement.  


## ⚠️ Security Considerations  
Blocking ports enhances security by:
- Reducing exposure to remote attacks.  
- Preventing unauthorized file-sharing and network access.  
- Limiting outbound connections that malware may exploit.

## Firewall Traffic Filtering
A firewall is a network security device or software that monitors and controls incoming and outgoing network traffic based on predetermined security rules. It acts as a barrier between a trusted internal network and untrusted external networks, such as the internet.
   # How Firewalls Filter Traffic:
      - Packet Filtering: Examines data packets against predefined rules (source/destination IP, ports, protocols) and allows or blocks them accordingly.
      - Stateful Inspection: Tracks the state of active connections and makes dynamic filtering decisions based on context.
      - Proxy Filtering: Intercepts and inspects traffic at an application layer, acting as a gateway between networks.
      - Deep Packet Inspection (DPI): Analyzes the content of data packets to detect malware, unauthorized access, or violations of security policies.
      - Rule-Based Control: Administrators configure policies that define which traffic should be allowed or denied based on various attributes.
      
By implementing firewall filtering mechanisms, networks can prevent unauthorized access, mitigate cyber threats, and ensure secure communication.


### 📜 Conclusion  
This project successfully demonstrates firewall rule configuration, testing, and documentation. The setup enhances network security while maintaining necessary functionalities.  

---
