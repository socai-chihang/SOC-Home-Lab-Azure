# 🛡️ SOC Home Lab – Azure + Microsoft Sentinel

This project is a hands-on cybersecurity lab simulating a Security Operations Center (SOC) environment using Microsoft Azure and Microsoft Sentinel. It’s designed to help practice threat detection, log analysis, and incident response.

---

## 🔧 Lab Architecture

- **Azure Virtual Machines**: Windows + Linux VMs for endpoint simulation
- **Microsoft Sentinel**: SIEM platform to collect, analyze, and respond to security events
- **Log Sources**: Sysmon, Security Logs, Azure Activity Logs
- **Kusto Query Language (KQL)**: Used for queries, alerts, and hunting
- **Python**: For automating log collection and writing custom enrichment scripts

---

## 🎯 Goals of the Lab

- Simulate real-world attacks (brute force, malware, etc.)
- Write and test analytic detection rules in Sentinel
- Practice incident investigation using KQL queries
- Create workbooks and dashboards for visualization
- Automate response using Sentinel playbooks (Logic Apps)

---

## 🧪 Lab Setup Summary

1. Provision VMs in Azure
2. Install **Sysmon** and configure logging
3. Connect to **Log Analytics Workspace**
4. Set up **Sentinel**
5. Enable and configure **data connectors**
6. Simulate attacks using test scripts (e.g., Brute Force, PowerShell abuse)
7. Query and analyze alerts in Sentinel

---

## 📸 Screenshots
> _(You can upload screenshots here later using drag-and-drop in GitHub!)_

---

## 📁 Files/Resources To Be Added
- `KQL-detection-rules/`
- `playbooks/`
- `log-samples/`
- `scripts/` (Python tools)

---

## 👨‍💻 Author
**Chi Hang**  
GitHub: [socai-chihang](https://github.com/socai-chihang)

---

## 🏁 Future Plans
- Integrate Defender for Endpoint
- Add threat intelligence feeds
- Explore automation with Logic Apps and Azure Functions
- Use AI to auto-label or prioritize alerts
