# Azure-Purple-Team-SOC-Lab

## Overview
This project is a Purple Team SOC lab built in Microsoft Azure. It simulates identity-based attacks, detects malicious activity using Microsoft Sentinel, and automates incident response workflows to replicate real-world SOC operations.

The lab focuses on cloud identity security, SIEM detection engineering, and automated response using a full attack → detect → respond → improve cycle.



## Architecture

<img width="4815" height="404" alt="mermaid-diagram (2)" src="https://github.com/user-attachments/assets/f9f6a60c-0d7f-4e83-ad70-e59e27b03733" />

## Attack Scenarios (Red Team)

- Password spray and brute-force attempts against Azure identities  
- Suspicious sign-in activity (impossible travel, unfamiliar IPs, anomalous location)  
- Unauthorized or excessive access to Azure Blob Storage containing sensitive data  
- Scripted or LLM-assisted generation of adversary scenarios mapped to MITRE ATT&CK  

---

## Detection Engineering (Blue Team)

- Built Microsoft Sentinel analytics rules using KQL to detect identity-based threats  
- Monitored Azure Entra ID sign-in logs, storage access logs, and VM telemetry  
- Correlated multi-source logs for full attack visibility  
- Mapped detections to MITRE ATT&CK cloud techniques  
- Tuned detection rules to reduce false positives and improve accuracy  

---

## Incident Response (Purple Team)

- Investigated alerts using Microsoft Sentinel incident workflows  
- Built and tested SOAR playbooks using Azure Logic Apps  
- Simulated SOC response actions including:
  - User account disablement  
  - IP blocking via network controls  
  - Alert escalation and notification workflows  
- Iteratively improved detection logic based on investigation results  

---

## Technologies Used

- Microsoft Sentinel (SIEM + SOAR)  
- Microsoft Entra ID (Identity & Access Management)  
- Microsoft Defender for Cloud  
- Azure Virtual Machines  
- Azure Blob Storage  
- Log Analytics Workspace  
- Kusto Query Language (KQL)  
- Azure Logic Apps  
- MITRE ATT&CK framework alignment  
- Optional: LLM-assisted adversary emulation for scenario generation  

---

## Key Outcomes

- Simulated a full SOC workflow from attack detection to automated response  
- Developed cloud-based detection rules using real Azure telemetry sources  
- Implemented MITRE ATT&CK-aligned detection engineering practices  
- Improved understanding of identity-based threats in cloud environments  
- Demonstrated SOC automation using SOAR playbooks  
- Practiced detection tuning and alert optimization techniques  

---

## Challenges & Learnings

- Designing realistic identity-based attack simulations without relying on traditional Active Directory  
- Building effective KQL queries that balance detection accuracy and false positives  
- Correlating logs across multiple Azure services for complete incident visibility  
- Translating raw telemetry into actionable SOC incidents in Microsoft Sentinel  
- Understanding the importance of detection tuning and alert fatigue reduction  

---

## Key Takeaway

This lab demonstrates a full cloud-native Purple Team lifecycle:

**Attack → Detect → Investigate → Respond → Improve**
