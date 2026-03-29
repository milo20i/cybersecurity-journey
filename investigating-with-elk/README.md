# Investigating with ELK — TryHackMe

## Overview

This lab focuses on using the **ELK Stack (Elasticsearch, Logstash, Kibana)** for log analysis and security monitoring.

The objective was to understand how security analysts use ELK to investigate logs and detect suspicious activity within an organization.

---

## ELK Stack Components

The ELK stack consists of three main components:

- **Elasticsearch** → stores and indexes large volumes of data  
- **Logstash** → collects and processes logs  
- **Kibana** → visualizes and analyzes data  

Together, they provide a powerful platform for **Security Information and Event Management (SIEM)**.

---

## Lab Scenario

In this lab, I took the role of a **SOC Analyst** and analyzed VPN logs to identify potential suspicious activity.

The investigation involved:

- Searching through large volumes of logs  
- Identifying anomalies in VPN connections  
- Correlating events to detect unusual behavior  

---

## Key Concepts Learned

### Log Collection and Parsing

Understanding how logs are collected and structured is essential for effective analysis.

Logs provide critical visibility into system and network activity.

---

### Searching and Filtering

Kibana allows powerful queries to filter logs and find relevant events quickly.

Example use cases:

- filtering by IP address  
- searching by timestamp  
- identifying repeated login attempts  

---

### Visualization and Dashboards

Kibana dashboards provide a **single pane of glass** to monitor activity.

Visualizations help identify:

- spikes in activity  
- unusual access patterns  
- potential security incidents  

---

### SOC Analyst Mindset

This lab emphasized the importance of:

- thinking like a defender  
- analyzing patterns instead of single events  
- correlating multiple data points  

---

## What I Learned

Working with ELK showed how important **log visibility and analysis** are in cybersecurity.

Even large datasets can be effectively analyzed using the right tools and techniques.

This lab helped me understand how SOC analysts detect threats and investigate real-world scenarios.

---

## Platform

Practice completed on **TryHackMe**.

This repository documents my journey into cybersecurity, covering both offensive and defensive security skills.
