
---

# 📄 4. `INC-004-Suspicious-powershell.md`

```md
# Incident Report: Suspicious PowerShell Activity

## Incident ID
INC-004

## Detection Title
PowerShell Execution Activity

## Severity
Medium

## Description
PowerShell activity was detected on the Windows system. While PowerShell is a legitimate administrative tool, suspicious or unauthorized commands may be used for execution, discovery, persistence, or other malicious activity.

## Detection Method
The activity was detected using Splunk by monitoring Windows Event IDs 4688 and 4104 and searching for PowerShell-related processes or commands.

## Detection Query

```spl
source="splunk_security_logs_50_with_description.csv"
index="main" (event_id=4688 OR event_id=4104)| 
search (process_name="*powershell*" OR cmd_line="*powershell*")|
table _time,user_name,process_name,parent_process,cmd_line|
sort _time
```
