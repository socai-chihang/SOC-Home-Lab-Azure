# 🛡️ SOC-Home-Lab-Azure: Getting Started

This document will guide you step-by-step to build a simulated SOC (Security Operations Center) lab in Microsoft Azure using Microsoft Sentinel. The lab is designed to practice detection, response, and automation in a cloud-based security environment.

---

## ✅ Overview

**Primary Goals:**
- Simulate common cyberattacks (e.g., brute force, malware)
- Ingest logs into Microsoft Sentinel
- Write KQL detection rules
- Practice alert triage and response
- Use Python/AI to automate parts of the workflow

---

## 🧭 Step-by-Step Roadmap

### 🟢 1. Lab Planning
- Define your use case: simulate attacker behaviors and test detections
- Draw the architecture: 1–2 VMs, Azure Sentinel, Log Analytics
- Tools needed: Azure Portal, Sentinel, Sysmon, KQL, Python

📝 Upload to GitHub:
- `notes/lab-setup.md` with goals, VM specs, and diagrams

---

### 🟡 2. Azure Environment Setup
- Provision Windows + Linux VMs
- Harden VMs (firewall rules, SSH/RDP)
- Install agents:
  - Windows: Sysmon
  - Linux: Auditd or Syslog
- Connect VMs to **Log Analytics Workspace**

📸 Upload to GitHub:
- `screenshots/vm-setup.png`
- `notes/agent-installation.md`

---

### 🔵 3. Enable Microsoft Sentinel
- Enable Sentinel in your Log Analytics Workspace
- Add data connectors:
  - Security Events
  - Azure Activity
  - Syslog
- Confirm log ingestion

📸 Upload to GitHub:
- `screenshots/sentinel-enabled.png`
- `notes/sentinel-data-sources.md`

---

### 🔴 4. Simulate Attacks
- Use simulated attack scripts or manual techniques:
  - Brute-force login
  - Suspicious PowerShell
  - Fileless malware
- Log and analyze attack behavior

📄 Upload to GitHub:
- `log-samples/brute-force.json`
- `notes/attack-scenarios.md`

---

### 🟣 5. Write Detection Rules (KQL)
- Use Sentinel Logs to write KQL queries
  - Detect failed logins
  - Detect suspicious process launches
- Turn into Analytics Rules

📄 Upload to GitHub:
- `kql-detection-rules/*.kql`
- `notes/creating-analytics-rules.md`

---

### 🟤 6. Automate Response (Optional)
- Build playbooks using Azure Logic Apps
- Example: email alert or isolate a VM on detection

📄 Upload to GitHub:
- `playbooks/email-alert-logicapp.json`
- `notes/response-playbooks.md`

---

### 🟢 7. Use Python Scripts (Optional)
- Write scripts to:
  - Parse Sentinel alerts
  - Enrich logs (e.g., geo-IP or threat intel lookups)

📝 Upload to GitHub:
- `scripts/parse-sentinel-alerts.py`
- `scripts/ip-checker.py`

---

## 🧠 Final Tips

- Take screenshots of dashboards and alerts
- Explain your thought process in `notes/` markdown files
- Keep each folder focused on one purpose (KQL, scripts, logs, etc.)

---

📁 [Back to the main README](../README.md)
