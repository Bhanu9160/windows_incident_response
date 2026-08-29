
# MITRE ATT&CK Mapping

This document maps the identified security incidents to the relevant MITRE ATT&CK techniques.

## Incident 1 – Brute Force

| Incident | Tactic            | Technique   | Technique ID | Description                                                                    |
| -------- | ----------------- | ----------- | ------------ | ------------------------------------------------------------------------------ |
| INC-001  | Credential Access | Brute Force | T1110        | Repeated authentication attempts are used to obtain valid account credentials. |

## Incident 2 – PowerShell Activity

| Incident | Tactic    | Technique  | Technique ID | Description                                                                 |
| -------- | --------- | ---------- | ------------ | --------------------------------------------------------------------------- |
| INC-002  | Execution | PowerShell | T1059.001    | PowerShell can be used to execute commands and scripts on a Windows system. |

## Incident 3 – Suspicious Process

| Incident | Tactic    | Technique                         | Technique ID | Description                                                                    |
| -------- | --------- | --------------------------------- | ------------ | ------------------------------------------------------------------------------ |
| INC-003  | Execution | Command and Scripting Interpreter | T1059        | Command or scripting interpreters may be used to execute commands on a system. |

## Incident 4 – Suspicious PowerShell

| Incident | Tactic    | Technique  | Technique ID | Description                                                                                 |
| -------- | --------- | ---------- | ------------ | ------------------------------------------------------------------------------------------- |
| INC-004  | Execution | PowerShell | T1059.001    | PowerShell may be used to execute suspicious or potentially malicious commands and scripts. |
