# Azure-SOC-Honeypot
Hands-on SOC project: Azure honeypot integrated with Sentinel, Defender for Endpoint and real attacker data analysis.

This project demonstrates a cloud-based Security Operations Center (SOC) lab that I designed and deployed using Microsoft Azure. The environment simulates real-world cyberattacks on a vulnerable Windows 10 honeypot, while integrating enterprise-grade security tools to detect, analyze, and respond to threats.

The goal of this project is to showcase practical, hands-on experience with:
	•	Threat detection and analysis using Microsoft Sentinel (SIEM).
	•	Endpoint protection and visibility with Microsoft Defender for Endpoint (MDE).
	•	Advanced event collection with Sysmon and Windows native logging.
	•	Offensive security simulation using Kali Linux for reconnaissance and attack testing.

⸻

⚙️ Lab Architecture
	•	Azure VM Honeypot (Windows 10) → Intentionally exposed RDP service to attract brute-force attempts.
	•	Microsoft Sentinel → Central SIEM for log ingestion, detection rules, and dashboards.
	•	Microsoft Defender for Endpoint → EDR integration for behavioral detection and timeline analysis.
	•	Sysmon + Windows Logs → Fine-grained event visibility (process creation, network connections, etc.).
	•	Kali Linux VM → Used to simulate attacker reconnaissance and exploitation techniques.

⸻

🔍 Key Features
	•	Real Attacker Data → Honeypot received 4,000+ brute-force login attempts, logged and analyzed in Sentinel.
	•	Custom Detection Rules → Built KQL queries to detect:
	•	RDP brute-force attempts
	•	Malware execution from suspicious .exe files
	•	Geo-IP Threat Mapping → Visualized attack origins across the globe.
	•	SOAR Playbooks → Automated email alerts triggered by Sentinel analytic rules.

⸻

📊 Screenshots & Evidence
	•	Sentinel dashboards (failed logins, attack timelines).
	•	Defender for Endpoint timeline analysis.
	•	KQL query outputs (detections).

⸻

🚀 Skills Demonstrated
	•	SIEM & SOC Operations → Log ingestion, correlation, and detection engineering.
	•	Threat Hunting → Identifying anomalous patterns such as beaconing intervals and brute-force campaigns.
	•	Incident Response → Following escalation workflows for suspicious executables 
	•	EDR Usage → Leveraging Defender for Endpoint for behavioral analysis.
	•	Red Team Awareness → Conducting recon/attack simulations for blue team validation.
