# Cybersecurity Analysis Report – Network Traffic & Phishing Investigation

## Overview
This repository contains two practical cybersecurity analysis projects focused on detecting network-based attacks and analyzing phishing campaigns. The work demonstrates a hands-on approach to threat detection, analysis, and mitigation.

---

## Project 1: Network Traffic Analysis – TCP SYN Scan Detection

### Objective
Analyze network traffic using Wireshark to identify suspicious behavior and detect potential attacks.

### Key Findings
- High volume of TCP SYN packets without completing the handshake
- Multiple RST/ACK responses from the target host
- Repeated connection attempts across multiple ports

### Conclusion
The observed behavior is consistent with a **TCP SYN Scan (half-open scan)**, commonly used during the reconnaissance phase of an attack.

### Attack Details
- **Attacker IP:** 192.168.200.100  
- **Target IP:** 192.168.200.150  

### Mitigation
- Block malicious IP at firewall level  
- Deploy IDS/IPS systems  
- Monitor abnormal traffic patterns  
- Apply service hardening  

### Tools Used
- Wireshark  

---

## Project 2: Phishing Campaign Analysis – CSIRT Italy (Trenitalia Scam)

### Objective
Analyze a phishing campaign reported by CSIRT Italy and understand its structure, risks, and mitigation strategies.

### Attack Scenario
The campaign impersonates Trenitalia and tricks users into completing a fake survey to obtain a reward.

### Attack Flow
1. Victim receives phishing email  
2. Redirected to fake survey page  
3. Promised reward (e.g., annual pass)  
4. Asked to provide personal and financial data  

### Impact
- Personal data theft  
- Financial fraud  
- Identity theft  

### Mitigation

#### Technical Controls
- Email filtering  
- SPF, DKIM, DMARC  
- URL/domain filtering  
- IDS/IPS deployment  

#### Organizational Measures
- Security awareness training  
- Phishing simulations  
- Incident reporting procedures  

#### User Awareness
- Avoid suspicious links  
- Verify sender identity  
- Do not share sensitive data  

### Threat Intelligence Context
This analysis follows the **Threat Intelligence Lifecycle**:
- Data collection  
- Analysis  
- Dissemination  

---

## Repository Structure
