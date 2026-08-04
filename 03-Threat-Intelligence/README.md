# 🔍 Threat Intelligence Integration – OilRig (APT34)

## Overview

This project demonstrates how open-source threat intelligence can be integrated into a SIEM platform to detect known malicious infrastructure.

The project focused on the Iranian threat actor OilRig (APT34). Open-source intelligence feeds were used to collect Indicators of Compromise (IOCs), which were then integrated into Wazuh using Constant Database (CDB) lists and custom detection rules.

---

## Objectives

- Research a real-world threat actor.
- Understand attacker behavior.
- Collect Indicators of Compromise.
- Build a Wazuh CDB list.
- Create IOC detection rules.
- Map detections to MITRE ATT&CK.

---

## Threat Actor

OilRig (APT34) is an Iranian state-sponsored Advanced Persistent Threat (APT) group known for targeting government, energy, financial, and telecommunications organizations, particularly within the Middle East.

The group commonly uses phishing campaigns, credential theft, PowerShell, web shells, and command-and-control infrastructure to compromise victim networks.

---

## Implementation

The project included:

- Researching OilRig using MITRE ATT&CK and AlienVault OTX.
- Collecting 10 Indicators of Compromise.
- Creating a Wazuh Constant Database list.
- Developing XML detection rules.
- Testing IOC matching within the Wazuh lab.

---

## Results

The IOC database and detection rules were successfully implemented within Wazuh. While testing revealed a telemetry configuration issue affecting Sysmon network events, the project provided valuable experience in operationalizing threat intelligence within a SIEM environment.

---

## Skills Gained

- Threat Intelligence
- IOC Collection
- MITRE ATT&CK
- AlienVault OTX
- CDB Lists
- XML Rules
- Detection Engineering

---

## Repository Contents

- OilRig Threat Profile
- IOC List
- Wazuh CDB List
- XML Detection Rules

---

## Project Screenshots

See the Images folder.
