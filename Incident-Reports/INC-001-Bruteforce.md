
Incident Report: Potential Brute Force Attack

## Incident ID

INC-001

## Detection Title

Potential Brute Force Login Attempt

## Severity

Medium

## Description

Multiple failed Windows login attempts were detected from the same source IP address targeting a user account. This activity may indicate a potential brute-force password attack.

## Detection Method

The activity was detected using Splunk by monitoring Windows Security Event ID 4625.

## Detection Query

```spl
source="splunk_security_logs_50_with_description.csv"  
index="main" event_id=4625| 
stats count by user_name,src_ip| 
where count >=5| 
sort - _time
```
