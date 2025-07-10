# Vulnerability Assessment & Packet Capture – Kali Linux

🔐 Built as part of my cybersecurity internship @ Uneeq Interns

This project performs a vulnerability assessment on a local target using Nmap, captures network traffic with tcpdump, and documents the entire process.

---

## 💡 Features

- ✅ Network discovery with Nmap  
- ✅ Port scanning and vulnerability detection  
- ✅ Packet capture during scanning using tcpdump  
- ✅ Detailed vulnerability report generation  
- ✅ Evidence collection with PCAP file and video walkthrough  

---

## 📸 Screenshots

<!-- Add your screenshots below like this -->

<img width="1570" height="892" alt="Screenshot 2025-07-10 180605" src="https://github.com/user-attachments/assets/ea406806-982d-444b-ab55-ebd7cae9b778" />
<img width="1548" height="896" alt="Screenshot 2025-07-10 180830" src="https://github.com/user-attachments/assets/fe86c149-82ec-4df5-b830-c0410d193021" />
<img width="1583" height="899" alt="Screenshot 2025-07-w10 180641" src="https://github.com/user-attachments/assets/78235b64-c965-417b-a2f5-5e40ee3692be" />
<img width="524" height="401" alt="Screenshot 2025-07-10 180641" src="https://github.com/user-attachments/assets/f7612610-31a0-4a67-9523-69c99a63e5d3" />
<img width="1577" height="853" alt="Screenshot 2025-07-10 180926" src="https://github.com/user-attachments/assets/2f5b239e-2aca-438c-887d-eda1ceb8936d" />


---

## 🎥 Walkthrough Video  
[Watch on YouTube](https://youtu.be/YOUR_VIDEO_LINK_HERE)

---

## 🔧 Tech Stack

- Nmap (Network Mapper)  
- tcpdump (Packet sniffer)  
- Kali Linux (Penetration testing OS)  
- Metasploitable VM (Vulnerable target)  
- VMware Workstation (Virtualization environment)  

---
🧩 Methodology and Steps
1. Network Discovery
bash
Copy
Edit
nmap -sn 192.168.0.0/24
Scanned subnet for active hosts

Identified target IP: 192.168.0.10 (Metasploitable VM)

2. Port Scanning
bash
Copy
Edit
nmap -T4 192.168.0.10
Conducted an aggressive port scan

Found multiple open ports including: 21 (FTP), 22 (SSH), 23 (Telnet), 25 (SMTP), 80 (HTTP), 445 (SMB), 3306 (MySQL)

3. Vulnerability Scanning
bash
Copy
Edit
nmap --script vuln -oN nmap_vuln.txt 192.168.0.10
Ran Nmap vulnerability scripts to detect known CVEs

Generated nmap_vuln.txt report highlighting exploitable services and vulnerabilities

4. Packet Capture
bash
Copy
Edit
tcpdump -i eth0 -w uneeq-task1.pcap
Captured live network packets during scanning activities

5- Wireshark result analysis 

Saved 11 packets, capturing scan traffic for further analysis
## 🧠 Author

Fadl Mostafa Alaa
17 y/o Cybersecurity Intern from Egypt 🇪🇬  
Builder of: TruthLens, BioCode, SoulSpace  
Scholarship warrior | Legacy in progress
