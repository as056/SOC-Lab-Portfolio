# 🎯 Detection Engineering with Wazuh

## Overview

This project focuses on creating and testing custom detection rules in Wazuh. The goal was to understand how SIEM platforms analyze logs, correlate events, and generate alerts for suspicious activities.

Custom XML rules were developed to detect authentication failures, Sysmon events, and Indicators of Compromise (IOCs). Each rule was mapped to the MITRE ATT&CK framework where appropriate.

---

## Objectives

- Learn Wazuh rule syntax.
- Create custom XML detection rules.
- Understand decoders and rule inheritance.
- Map detections to MITRE ATT&CK.
- Test detections using generated events.

---

## Implementation

During this project I:

- Studied built-in Wazuh rules.
- Learned rule IDs and inheritance using `<if_sid>`.
- Created custom rules in `local_rules.xml`.
- Validated rules using `wazuh-logtest`.
- Tested authentication failures.
- Investigated alert generation.
- Troubleshot rule validation and matching issues.

---

## Detection Examples

Implemented detections included:

- Failed Windows logins
- Windows Event ID 4625
- Sysmon Process Creation
- Sysmon Network Connection
- Custom IOC detections
- MITRE ATT&CK mappings

---

## Results

Successfully created multiple custom detection rules that generated alerts for simulated security events. The project improved my understanding of detection engineering, rule logic, and event correlation.

---

## Skills Gained

- Detection Engineering
- XML
- Wazuh Rules
- Event Correlation
- MITRE ATT&CK
- Troubleshooting
- Security Monitoring

---

## Project Screenshots

See the Images folder.
