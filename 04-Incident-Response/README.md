# 🚨 Incident Response – SSH Brute Force Attack Simulation

## Project Overview

This project demonstrates a complete incident response workflow by simulating an SSH brute-force attack against a Linux system monitored by Wazuh.

The objective was to observe how an attack progresses through the cyber kill chain, collect evidence from security logs, investigate the generated alerts, and document the incident using standard SOC practices.

The project concluded with the creation of an Incident Report and an Incident Response Playbook.

---

# Objectives

The objectives of this project were to:

- Simulate an SSH brute-force attack.
- Monitor attack activity using Wazuh.
- Collect evidence from generated alerts.
- Build a timeline of attacker actions.
- Produce a professional Incident Report.
- Develop an Incident Response Playbook.

---

# Lab Environment

| Component | Description |
|-----------|-------------|
| Attacker Machine | Windows 10 (PowerShell SSH client) |
| Target Machine | Ubuntu Linux |
| Monitoring Platform | Wazuh SIEM |
| Authentication | OpenSSH |

---

# Attack Scenario

The attack simulation followed a simple but realistic sequence:

1. Multiple failed SSH login attempts.
2. Successful authentication using valid credentials.
3. Creation of a new user account on the target system.
4. Detection and investigation using Wazuh.

This scenario represents common post-compromise activities that SOC analysts investigate.

---

# Stage 1 – SSH Brute Force

Several failed login attempts were generated against the Ubuntu server.

Wazuh successfully detected the authentication failures and generated corresponding security alerts.


<img width="1365" height="419" alt="brute-force" src="https://github.com/user-attachments/assets/864e6d26-38e5-4c64-b882-c1afdd4a934b" />


---

# Stage 2 – Successful Login

After repeated failed attempts, a successful SSH login was performed.

This event marked the transition from attempted access to system compromise.


<img width="1360" height="48" alt="access " src="https://github.com/user-attachments/assets/be2de58f-279f-4940-b9e0-4f0be5d440d6" />


---

# Stage 3 – User Creation

Following successful access, a new Linux user account was created.

This activity represents a common persistence technique observed after initial access.


<img width="1363" height="66" alt="new user" src="https://github.com/user-attachments/assets/6b5796e4-6bef-4d87-99f6-05ceadbda4d5" />


---

# Investigation

The collected alerts were analyzed using the Wazuh Dashboard to determine:

- Attack timeline
- Source IP
- Target host
- Authentication events
- User activity

The investigation confirmed the complete attack sequence.


<img width="1361" height="568" alt="Screenshot 2026-08-06 003018" src="https://github.com/user-attachments/assets/7663d6c1-046d-4bf0-a3ca-2da0b478fbcf" />


---

# Attack Timeline

The following timeline illustrates the sequence of events observed during the simulated SSH brute-force attack. By correlating authentication logs and security alerts, Wazuh enabled the complete reconstruction of the attack from initial access attempts through post-compromise activity.

<img width="1672" height="941" alt="ChatGPT Image Aug 6, 2026, 10_24_15 PM" src="https://github.com/user-attachments/assets/811efe37-9d52-4904-a085-4a50a4d5ac08" />


---

# Incident Documentation

Following the investigation, two documents were produced:

- Incident Report
- Incident Response Playbook

These documents summarize the incident, affected assets, indicators, recommended remediation steps, and the standard response process for similar attacks.

Supporting Files:

- 📄 Incident-Report.pdf
- 📄 SSH-Bruteforce-Playbook.pdf

---

# Results

The project successfully demonstrated a complete incident response workflow from attack simulation through investigation and documentation.

The generated alerts provided sufficient evidence to reconstruct the attack timeline and understand each stage of the compromise.

---

# Skills Gained

- Incident Response
- Log Analysis
- Linux Security
- SSH Security
- Timeline Analysis
- Security Monitoring
- Alert Investigation
- Digital Evidence Collection
- Incident Documentation

---

# Key Takeaways

This project brought together the knowledge gained throughout the internship by applying SIEM monitoring, detection engineering, and log analysis to a realistic attack scenario.

Beyond identifying malicious activity, the exercise emphasized the importance of documenting incidents, reconstructing attack timelines, and following a structured incident response process similar to those used in Security Operations Centers (SOCs).
