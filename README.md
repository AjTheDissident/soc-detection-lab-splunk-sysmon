# 🛡️ SOC Detection Lab – Splunk + Sysmon + Kali Attack Simulation

## 🔍 Overview

This project is a Security Operations Center (SOC) lab designed to simulate real-world attacker behavior and detect it using Splunk SIEM and Sysmon telemetry.

The lab demonstrates how adversary activity is generated, collected, and analyzed using:

- Kali Linux (attacker machine)
- Windows 11 (target endpoint)
- Sysmon (endpoint monitoring)
- Splunk Enterprise (SIEM platform)

The goal is to simulate reconnaissance attacks and detect them using SIEM correlation rules mapped to MITRE ATT&CK.

---

## 🧱 SOC Architecture

```mermaid
flowchart LR
A[Kali Linux - Attacker] -->|Nmap Scan| B[Windows 11 - Target]
B -->|Sysmon Logs| C[Splunk SIEM]
C --> D[Detection Dashboard]
