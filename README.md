# Adaptive Honeypot Behavioral Attack Dataset

## Overview

This dataset contains behavioral cybersecurity telemetry collected from a Cowrie SSH/Telnet honeypot deployed in a controlled virtualized environment.

The dataset was generated through simulated cyberattack interactions including reconnaissance, malware staging, privilege escalation, persistence attempts, and destructive attack behavior.

It is designed for:
- Intrusion Detection Systems (IDS)
- Cybersecurity Machine Learning
- Behavioral Threat Analysis
- Ensemble Learning Research
- Honeypot Telemetry Analysis

---

# Dataset Features

| Feature | Description |
|---|---|
| timestamp | Event timestamp |
| eventid | Cowrie event type |
| src_ip | Attacker source IP |
| session | Unique session identifier |
| username | Attempted username |
| password | Attempted password |
| command | Executed command |
| protocol | Network protocol |
| recon_activity | Reconnaissance behavior flag |
| malware_activity | Malware activity flag |
| privilege_escalation | Privilege escalation indicator |
| destructive_behavior | Destructive attack indicator |
| persistence_behavior | Persistence mechanism indicator |
| command_length | Length of executed command |
| failed_command | Failed command indicator |
| severity | Attack severity label |

---

# Attack Categories Included

The dataset includes telemetry from:

- Brute-force attacks
- Reconnaissance activities
- Malware download attempts
- Payload execution
- Privilege escalation
- Persistence attempts
- Destructive commands
- Failed attack attempts

Example attack commands:

```bash
wget payload.sh
chmod +x payload.sh
./payload.sh

rm -rf /
dd if=/dev/zero of=/dev/sda
```

---

# Severity Labels

The dataset contains multi-class threat labels:

| Label | Description |
|---|---|
| Normal | Benign activity |
| Low | Reconnaissance behavior |
| Medium | Malware staging activity |
| High | Privilege escalation / persistence |
| Critical | Destructive attack behavior |

---

# Dataset Format

- Format: CSV
- Source: Cowrie Honeypot Logs (JSON → CSV)
- Generated using custom Python preprocessing pipeline

---

# Applications

This dataset can be used for:

- Machine Learning-based IDS
- Threat Classification
- Anomaly Detection
- Behavioral Security Analytics
- Ensemble Learning Research
- Cyber Threat Intelligence

---

# Environment

- Kali Linux
- VMware Workstation
- Cowrie Honeypot
- Python
- Scikit-learn
- XGBoost

---

# Important Note

This dataset was generated in a safe and isolated virtual environment strictly for:
- academic research,
- cybersecurity experimentation,
- ethical hacking education.

No real systems were harmed during attack simulation.
