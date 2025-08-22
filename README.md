# SIEM-with-Splunk
Simple SIEM lab using Splunk for log ingestion and alerting
#Splunk Blue Team Lab

This is my beginner-friendly SIEM lab using **Splunk** to simulate log ingestion, create alerts, and practice basic threat detection—focusing on core skills needed for a Blue Team cybersecurity role.

---

### Objectives

- Learn how to install and configure Splunk in a test environment  
- Ingest Windows and Linux logs into Splunk  
- Create dashboards and alerts to detect unusual behavior  
- Understand basic incident response using log analysis

---

###  Lab Setup

| Component         | Description                              |
|------------------|------------------------------------------|
| **Splunk Free**   | Installed on Windows or Ubuntu VM        |
| **Log Sources**   | Windows 10 logs, Sysmon, Ubuntu syslog   |
| **Network**       | Local-only VirtualBox lab with NAT       |

---

###  Sample Use Cases

- Detect failed login attempts from unknown IPs
- Monitor USB device connections (via Windows logs)
- Alert on PowerShell usage or suspicious command-line activity
- Track system reboots and privilege escalations

---

###  Folder Structure

```plaintext
splunk-blue-team-lab/
├── installation-guides/
│   ├── install-splunk-windows.md
│   └── install-splunk-ubuntu.md
├── inputs-config/
│   └── inputs.conf (Sysmon, Windows Logs, etc.)
├── sample-alerts/
│   └── excessive-failed-logins.md
└── dashboards/
    └── windows-activity-overview.json
```

---

###  Resources I'm Using

- [Splunk Fundamentals 1 (Free Course)](https://www.splunk.com/en_us/training.html)
- [Windows Event IDs Cheat Sheet](https://www.ultimatewindowssecurity.com/securitylog/encyclopedia/)
- [TryHackMe – SOC Level 1](https://tryhackme.com/room/blueprimer)

---

###  Tools

- Splunk Free Edition (local)
- Windows Sysmon + Event Viewer
- Ubuntu rsyslog
- MITRE ATT&CK for detection mapping

---

> "Logs tell a story—my job is to read between the lines."
