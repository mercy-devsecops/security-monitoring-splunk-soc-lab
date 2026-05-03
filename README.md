# 🛡️ Security Monitoring & SOC Simulation with Splunk

## 📌 Overview

This project simulates a real-world Security Operations Center (SOC) environment using Splunk as a SIEM platform.
It demonstrates log ingestion, threat detection, attack simulation, and security analytics across multiple virtual machines.

The system includes Ubuntu Server, Windows 11 Lab, and Kali Linux to simulate real attacker–defender scenarios.

---

## 🧱 Architecture

* **Ubuntu Server** → Splunk Enterprise (SIEM + log analysis)
* **Windows 11 VM** → Log forwarder (System, Security, Application, Sales logs)
* **Kali Linux VM** → Attack simulation (brute force, SSH attacks)
* **Splunk Universal Forwarder** → Log shipping agent

---

## ⚙️ Splunk Index Design

* `web` → Apache/Nginx logs
* `auth` → Linux authentication logs
* `wineventlog` → Windows event logs
* `sales` → simulated e-commerce logs
* `web_traffic` → performance monitoring
* `attacks` → security attack simulation logs

---

## 🔐 Key Security Use Cases Implemented

### 1. Brute Force Detection

Detected IPs exceeding 10 failed login attempts within 1 minute window.

### 2. Authentication Monitoring

Tracked failed vs successful SSH login attempts for users like `admin_user` and `jdoe`.

### 3. Attack Simulation (Kali Linux)

Simulated SSH brute-force attacks against Ubuntu VM and analyzed logs in Splunk.

### 4. Geo-IP Threat Analysis

Mapped malicious IPs to geographic locations using `iplocation`.

### 5. E-commerce Fraud Analysis

Identified top customers based on revenue using Splunk stats aggregation.

---

## 📊 SPL Use Case Examples

* Failed login detection
* Error monitoring in internal logs
* Time-based performance analysis
* Event correlation using `transaction`
* Lookup-based threat intelligence matching

---

## 🖥️ Infrastructure

* 3 Virtual Machines:

  * Ubuntu Server (Splunk SIEM)
  * Windows 11 (Log Forwarder)
  * Kali Linux (Attack Simulation)

---

## 📈 Skills Demonstrated

* SIEM configuration (Splunk)
* Log ingestion & forwarding
* Threat detection engineering
* SPL query writing
* Attack simulation (ethical hacking lab)
* SOC workflow design

---

## 📄 Status

🟡 In Progress (70% complete)
🎯 Expected completion: End of month

Remaining:

* Screenshot documentation
* Final dashboard polishing
