
# Incident Report: Suspicious Account Creation

## Incident ID

INC-002

## Detection Title

New Windows Account Creation

## Severity

Medium

## Description

A new Windows user account was created on the system. Unauthorized account creation may indicate persistence, unauthorized access, or suspicious administrative activity.

## Detection Method

The activity was detected using Splunk by monitoring Windows Security Event ID 4720.

## Detection Query

```spl
source="splunk_security_logs_50_with_description.csv"  
index="main" event_id=4720| 
table _time,user_name,workstation| 
sort _time
```
