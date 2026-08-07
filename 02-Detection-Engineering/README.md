# 🎯 Detection Engineering with Wazuh

## Project Overview

After deploying the Wazuh SIEM lab, the next step was to understand how security detections are created and customized. This project focused on detection engineering by developing custom Wazuh XML rules to identify suspicious activities and generate meaningful alerts.

Throughout the project, I explored Wazuh's rule hierarchy, event correlation, and MITRE ATT&CK mapping while troubleshooting real-world configuration issues encountered during rule development.

---

# Objectives

The objectives of this project were to:

- Understand how Wazuh processes security events.
- Learn the structure of Wazuh XML rules.
- Create custom detection rules using `local_rules.xml`.
- Extend existing Wazuh rules using rule inheritance (`<if_sid>`).
- Validate and test custom detections.
- Map detections to the MITRE ATT&CK framework.

---

# Lab Environment

| Component | Description |
|-----------|-------------|
| SIEM Platform | Wazuh |
| Endpoint | Windows 10 |
| Log Source | Windows Security Logs & Sysmon |
| Rule Engine | local_rules.xml |
| Framework | MITRE ATT&CK |

---

# Rule Development

The project began by studying Wazuh's built-in rules to understand how alerts are generated.

I learned how to:

- Create custom XML rules
- Assign rule IDs
- Set severity levels
- Extend built-in rules using `<if_sid>`
- Match specific event fields
- Organize rules into custom groups

The following image shows one of the custom rules developed during this project.

<img width="1287" height="596" alt="custom rule" src="https://github.com/user-attachments/assets/042e83e3-0b1b-4172-af26-c832f74591d0" />


---

# Authentication Detection

A custom detection rule was created to identify failed Windows login attempts by extending the built-in authentication rule.

The rule was tested by intentionally entering incorrect credentials on the Windows endpoint.


Once the authentication event was generated, the custom rule successfully produced a high-severity alert.

<img width="1366" height="719" alt="failed login alert" src="https://github.com/user-attachments/assets/6581040c-5f4b-472b-9163-f682496c93dc" />


---

# Sysmon Event Monitoring

To expand detection capabilities, Sysmon logging was integrated into the lab.

Custom rules were developed to monitor Sysmon Event ID 3 (Network Connections), providing the foundation for future IOC-based detections.

Although telemetry inconsistencies prevented complete testing, the project provided valuable experience in working with Sysmon events inside Wazuh.


<img width="1364" height="594" alt="sysmon ID 3" src="https://github.com/user-attachments/assets/fa158fde-5849-4464-8bb5-5ba614916d67" />


---

# Rule Validation

Each custom rule was validated after deployment to ensure it was successfully loaded by the Wazuh Manager before testing.

This validation process helped identify configuration issues such as duplicate rule IDs, incorrect XML structure, and field mismatches.

<img width="1366" height="652" alt="rule validation" src="https://github.com/user-attachments/assets/e5b683a5-7589-4c66-9a63-952d383c1ec1" />


---

# Challenges Encountered

Several issues were encountered during development, including:

- Invalid XML structure
- Duplicate rule IDs
- Username field mismatches
- Incorrect field names
- Sysmon telemetry inconsistencies

Resolving these issues significantly improved my understanding of Wazuh's rule processing, event decoding, and troubleshooting methodology.

---

# Results

By the end of the project, I successfully:

- Created custom Wazuh detection rules.
- Extended built-in Wazuh rules using inheritance.
- Detected Windows authentication failures.
- Implemented Sysmon-based detections.
- Learned the complete lifecycle of developing, testing, and troubleshooting detection rules.

---

# Skills Gained

- Detection Engineering
- XML Rule Development
- Windows Event Analysis
- Sysmon
- Event Correlation
- MITRE ATT&CK
- Security Monitoring
- Troubleshooting

---

# Key Takeaways

This project provided hands-on experience in detection engineering by moving beyond default SIEM capabilities and developing custom security detections. It also highlighted the importance of validating event collection and understanding the relationship between log sources, decoders, and detection rules before implementing advanced analytics.
