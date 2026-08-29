
---

# 📄 3. `INC-003-Privilege.md`

```md
# Incident Report: Suspicious Privilege Activity

## Incident ID
INC-003

## Detection Title
Privilege or Group Membership Change

## Severity
High

## Description
Privilege-related activity was detected on the Windows system. This includes special privileges assigned during logon or changes to security-enabled groups. Unexpected privilege changes may indicate privilege escalation or unauthorized administrative activity.

## Detection Method
The activity was detected using Splunk by monitoring Windows Security Event IDs 4672, 4728, and 4732.

## Detection Query

```spl
source="splunk_security_logs_50_with_description.csv"  
index="main"  (event_id=4672 OR event_id=4728 OR event_id=4732)|
table _time,user_name,workstation,event_id,logon_type,description|
sort _time
```
