Windows Incident Response

📌 Project Overview

Windows Incident Response is a cybersecurity project focused on detecting, documenting, and analyzing suspicious activities on Windows systems.

The project demonstrates a structured incident response workflow using security incidents, detection queries, Windows logs, and MITRE ATT&CK mapping.

🎯 Objectives

- Detect suspicious activities on Windows systems.
- Document security incidents in a structured format.
- Analyze relevant Windows security logs.
- Create detection queries for identifying suspicious behavior.
- Map detected activities to MITRE ATT&CK techniques.
- Provide a foundation for further incident investigation.

📂 Project Structure

windows_incident_response/
│
├── incidents/
│   ├── INC-001-Brute-Force.md
│   ├── INC-002-PowerShell.md
│   ├── INC-003-Suspicious-Process.md
│   └── INC-004-Suspicious-Powershell.md
│
├── detection-queries/
│   └── detection-queries.md
│
├── logs/
│   └── security-logs.csv
│
├── mitre-mapping/
│   └── attack-mapping.md
│
└── README.md

🚨 Incidents Covered

INC-001 – Brute Force

Focuses on repeated failed authentication attempts that may indicate an attempt to gain unauthorized access.

INC-002 – PowerShell

Focuses on PowerShell activity that may indicate suspicious command or script execution.

INC-003 – Suspicious Process

Focuses on unusual or potentially suspicious process activity on a Windows system.

INC-004 – Suspicious PowerShell

Focuses on suspicious PowerShell commands or scripts that may require further investigation.

🔍 Detection Queries

Detection queries are used to identify suspicious activities from Windows security events and logs.

The project includes detection logic for:

- Repeated failed login attempts
- PowerShell activity
- Suspicious processes
- Suspicious PowerShell execution

📊 Logs

The "logs" directory contains security log data associated with the documented incidents.

These logs provide evidence for identifying and analyzing suspicious activities.

🛡️ MITRE ATT&CK Mapping

The identified activities are mapped to relevant MITRE ATT&CK techniques.

Incident| Technique| ID
Brute Force| Brute Force| T1110
PowerShell| PowerShell| T1059.001
Suspicious Process| Command and Scripting Interpreter| T1059
Suspicious PowerShell| PowerShell| T1059.001

🔎 Investigation

The next stage of the project is to investigate the detected activities using the available logs and detection results.

Investigation may include:

- Reviewing related events
- Identifying affected users
- Analyzing processes
- Reviewing timestamps
- Correlating security events
- Determining whether activity is malicious or legitimate

🧰 Technologies & Concepts

- Windows Security Logs
- Incident Response
- Threat Detection
- Detection Queries
- MITRE ATT&CK
- Security Operations (SOC)
- PowerShell
- Windows Event Analysis
