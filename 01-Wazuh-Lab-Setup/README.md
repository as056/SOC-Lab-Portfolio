# 🛡️ Wazuh SIEM Lab Setup

## Overview

This project documents the deployment and configuration of a Security Information and Event Management (SIEM) laboratory using Wazuh. The lab was developed during my cybersecurity internship to gain practical experience in centralized log collection, security monitoring, threat detection, and incident investigation.

The environment consists of an Ubuntu Server hosting the Wazuh Manager, Indexer, and Dashboard, along with Windows and Linux endpoints configured to forward security logs to Wazuh.

---

## Objectives

- Deploy a functional Wazuh SIEM environment.
- Configure centralized log collection.
- Connect Windows and Linux endpoints.
- Monitor security events in real time.
- Understand SIEM architecture and SOC workflows.

---

## Lab Environment

| Component | Purpose |
|----------|----------|
| Ubuntu Server | Hosts Wazuh Manager, Indexer, and Dashboard |
| Windows 10 | Monitored endpoint running the Wazuh Agent |
| Ubuntu Client | SSH attack simulation |
| VMware Workstation | Virtualization platform |

---

## Architecture

```
Windows Endpoint
        │
        │
Ubuntu Client (SSH)
        │
        ▼
Ubuntu Server
 ├── Wazuh Manager
 ├── Wazuh Indexer
 └── Wazuh Dashboard
```

---

## Implementation

During the setup process, I:

- Installed Ubuntu Server.
- Installed the Wazuh Stack.
- Enrolled Windows and Linux agents.
- Verified communication between agents and manager.
- Confirmed event collection.
- Explored dashboards and MITRE ATT&CK mapping.

---

## Results

The SIEM environment successfully collected and analyzed logs from multiple endpoints. Security events were visualized through the Wazuh Dashboard, enabling centralized monitoring and investigation.

---

## Skills Gained

- SIEM Deployment
- Linux Administration
- Windows Event Monitoring
- Wazuh Administration
- Agent Management
- Log Collection
- VMware

---

## Project Screenshots

See the **Images** folder for screenshots demonstrating the deployment and operation of the SIEM lab.
