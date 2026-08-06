# 🔍 Threat Intelligence Integration – OilRig (APT34)

## Project Overview

This project focused on integrating open-source threat intelligence into the Wazuh SIEM platform. The objective was to research a real-world threat actor, collect publicly available Indicators of Compromise (IOCs), and use them to build custom IOC-based detections within Wazuh.

OilRig (APT34), a threat group known for targeting organizations in the Middle East, was selected due to its relevance to the GCC region.

---

# Objectives

The objectives of this project were to:

- Research a real-world threat actor.
- Understand attacker tactics and techniques.
- Collect Indicators of Compromise (IOCs).
- Create a Wazuh Constant Database (CDB).
- Develop custom IOC detection rules.
- Map detections to the MITRE ATT&CK framework.

---

# Threat Actor Research

Research was conducted using trusted open-source intelligence sources including:

- MITRE ATT&CK
- AlienVault OTX
- Check Point Research

The collected information provided insight into OilRig's targeting, malware families, campaigns, and attack techniques.

![OilRig Research](apt34-research.png)

---

# IOC Collection

Ten Indicators of Compromise were collected, including:

- IPv4 addresses
- Domains
- File hashes

The IOC list was organized into a dedicated text file for future reference and integration.

📄 **Supporting file:** `oilrig_iocs.txt`


<img width="569" height="356" alt="iocs" src="https://github.com/user-attachments/assets/a6a77fb2-3928-42cb-a5cd-a62989d79e3c" />


---

# Building the Wazuh CDB

The collected IOCs were converted into a Wazuh Constant Database (CDB) format to enable automated IOC matching.

The resulting CDB became the foundation for custom threat intelligence detections.


<img width="825" height="288" alt="CDB list" src="https://github.com/user-attachments/assets/3466ea42-15d4-4a9d-9447-fde4be8066d8" />

---

# Custom IOC Detection Rules

Custom XML rules were developed to compare incoming Sysmon network connection events against the OilRig IOC database.

The rules were designed to detect outbound communication with known malicious infrastructure.




<img width="909" height="697" alt="IOC rule" src="https://github.com/user-attachments/assets/92fc9e1a-d4fb-43d0-9899-479574f44bd8" />


---

# MITRE ATT&CK Mapping

OilRig techniques were reviewed using the MITRE ATT&CK framework to better understand how the group's behavior aligns with attacker tactics and techniques.

This helped ensure that the detection logic reflected documented adversary behavior.

<img width="1366" height="613" alt="Oilrig TTPs" src="https://github.com/user-attachments/assets/9411a3a4-40e9-4aed-9e82-711a7bbf5b7e" />


---

# Challenges Encountered

The primary challenge during this project involved inconsistent Sysmon Event ID 3 telemetry reaching Wazuh.

Although the IOC database and detection rules were correctly configured, the required network connection events were not consistently available for matching.

This highlighted the importance of validating log collection before implementing advanced detection logic.

---

# Results

The project successfully produced:

- A threat actor profile
- A structured IOC database
- A Wazuh CDB list
- Custom IOC detection rules
- MITRE ATT&CK mappings

These components demonstrated how threat intelligence can be operationalized within a SIEM environment to support proactive threat detection.

---

# Skills Gained

- Threat Intelligence
- IOC Collection
- MITRE ATT&CK
- Wazuh CDB Lists
- XML Rule Development
- Detection Engineering
- Security Research
- Threat Hunting Concepts

---

# Supporting Files

- 📄 OilRig-Threat-Profile
- 📄 oilrig_iocs.txt


---

# Key Takeaways

This project demonstrated how publicly available threat intelligence can be transformed into actionable detections within a SIEM platform. Beyond collecting IOCs, I learned how to structure threat intelligence, integrate it into Wazuh, and build detections that align with real-world adversary behavior.
