# 🛡️ Wazuh SIEM Lab Setup

## Project Overview

As part of my cybersecurity internship, I designed and deployed a Security Information and Event Management (SIEM) laboratory using **Wazuh**. The objective was to build a centralized security monitoring environment capable of collecting logs from multiple endpoints, detecting security events, and supporting incident investigation.

The lab served as the foundation for all subsequent projects in this portfolio, including custom detection engineering, threat intelligence integration, incident response, and security dashboard development.

---

# Objectives

The primary objectives of this project were to:

- Deploy a fully functional Wazuh SIEM environment.
- Configure centralized log collection from Windows and Linux endpoints.
- Understand the architecture and components of a SIEM platform.
- Monitor security events through the Wazuh Dashboard.
- Prepare a lab environment for future detection engineering and incident response exercises.

---

# Lab Environment

| Component | Description |
|-----------|-------------|
| Hypervisor | VMware Workstation |
| SIEM Server | Ubuntu Server |
| SIEM Platform | Wazuh Manager, Indexer, Dashboard |
| Windows Endpoint | Windows 10 with Wazuh Agent |
| Linux Endpoint | Ubuntu VM used for SSH attack simulations |

---

# Lab Architecture

The following diagram illustrates the overall architecture of the lab environment.

<img width="920" height="544" alt="Lab architecture" src="https://github.com/user-attachments/assets/2449d126-d26e-4091-a928-5edc5c1922f5" />


The Ubuntu server hosts the Wazuh Stack, while both Windows and Linux endpoints forward security events to the Wazuh Manager for analysis.

---

# Wazuh Deployment

The Wazuh platform was successfully deployed on Ubuntu Server, including:

- Wazuh Manager
- Wazuh Indexer
- Wazuh Dashboard

After installation, the web dashboard became the central interface for monitoring alerts, connected agents, security events, and MITRE ATT&CK mappings.

<img width="1366" height="601" alt="Dashboard" src="https://github.com/user-attachments/assets/81479ace-1127-48ec-a8f6-60f9862d37c1" />


---

# Endpoint Enrollment

A Windows endpoint and a Linux endpoint were enrolled into the Wazuh Manager using Wazuh Agents.

After registration, both endpoints successfully communicated with the manager, allowing security logs to be collected and analyzed centrally.

<img width="1366" height="763" alt="agent" src="https://github.com/user-attachments/assets/6641db54-6966-4dbc-a001-65a9c25d4adb" />


---

# Security Monitoring

Once the endpoints were connected, Wazuh began collecting security events in real time.

The dashboard provided visibility into:

- Security alerts
- Event severity
- Authentication activity
- Endpoint status
- MITRE ATT&CK mappings

<img width="1364" height="571" alt="alerts" src="https://github.com/user-attachments/assets/173acdd5-9949-4501-b91b-59ec074e1001" />


---

# MITRE ATT&CK Integration

One of Wazuh's key features is automatic mapping of alerts to the MITRE ATT&CK framework.

This functionality helped relate security events to known adversary tactics and techniques, providing additional context during investigations.

<img width="1366" height="634" alt="MITRE dashboard" src="https://github.com/user-attachments/assets/b99a892c-7cd1-4bc8-9f4f-f4ea6ba52729" />


---

# Challenges Encountered

During deployment, several configuration issues were encountered while integrating Windows event logs and Sysmon telemetry.

Troubleshooting these issues improved my understanding of:

- Windows Event Collection
- Wazuh Agent configuration
- Sysmon logging
- Event forwarding
- SIEM troubleshooting methodologies

Resolving these issues strengthened the reliability of the lab and prepared it for future detection engineering projects.

---

# Results

The project successfully produced a fully operational SIEM laboratory capable of:

- Collecting Windows and Linux security events
- Monitoring authentication activity
- Displaying alerts through the Wazuh Dashboard
- Supporting custom detection rules
- Supporting threat intelligence integration
- Supporting incident response investigations

The completed lab became the foundation for all subsequent cybersecurity projects completed during my internship.

---

# Skills Gained

- SIEM Deployment
- Wazuh Administration
- Linux Administration
- Windows Event Monitoring
- Agent Management
- Log Collection
- Security Monitoring
- VMware Virtualization
- Troubleshooting


# Key Takeaways

This project provided practical experience in deploying and administering a SIEM platform from the ground up. Beyond installation, it emphasized the importance of log collection, endpoint visibility, and troubleshooting data ingestion issues.

The completed lab became the foundation for implementing custom detection rules, integrating threat intelligence, simulating attacks, and performing incident response activities throughout the internship.
