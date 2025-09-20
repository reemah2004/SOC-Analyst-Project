Redline Stealer Traffic Analysis (Wireshark)  

This project simulates a "SOC analyst investigation" demonstrating detection of malicious traffic, C2 communication, and data exfiltration patterns using 
wireshark and Threat Intelligence tools.  

Project Overview  
The goal of this project was to replicate a real-world malware investigation workflow:  
- Identify suspicious DNS queries 
- Trace HTTP POST requests used for data exfiltration  
- Correlate TLS activity with sandbox evasion tactics  
- Extract Indicators of Compromise (IOCs)  
- Document findings in a professional Incident Response Report (Identification → Containment → Eradication → Recovery)  

Tools & Technologies  
- Wireshark – Network traffic capture & packet analysis  
- VirusTotal – IOC enrichment & validation  
- Windows/Linux test environment – Analysis workstation
  
Key Project Steps  
- DNS Query Analysis→ Identified suspicious request to `api.ip.sb`, used by malware to check external IPs  
- HTTP Traffic Analysis→ Traced multiple POST requests to `188.190.10.10`, confirming exfiltration activity  
- TLS Activity Review → Observed handshake with Cloudflare server, consistent with sandbox evasion behavior  
- C2 Indicators→ Structured XML payloads with gradually increasing sizes indicated staged data theft  
- Incident Response Reporting → Documented findings across Identification, Containment, Eradication, and Recovery phases  

Screenshots  
Screenshots are included inside the full report.  
DNS query to `api.ip.sb`  
HTTP POST requests to C2 (`188.190.10.10`)  
TLS handshake to Cloudflare server  
Wireshark packet captures of exfiltration patterns  

Full Report  
👉 [Download the Incident Report (PDF)](./Redline_Stealer_Incident_Report.pdf)  

Key Takeaways  
- Hands-on experience in malware traffic analysis & incident response  
- Improved ability to spot C2 communication and exfiltration patterns  
- Demonstrated use of packet analysis (Wireshark) for SOC workflows  
- Reinforced the importance of detecting and documenting exfiltration activity with IOCs  


#CyberSecurity #SOCAnalyst #BlueTeam #Wireshark #IncidentResponse #ThreatHunting
