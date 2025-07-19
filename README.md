 # 🔍 Security Event Analysis Using Splunk SIEM

## 📖 Overview

This project explores how Security Information and Event Management (SIEM) tools, specifically **Splunk**, can be used to monitor and investigate suspicious activities through simulated log data. The goal was to detect incidents like failed login attempts, brute-force behavior, malware infections, and risky IP-user associations by building and running meaningful queries.

---

## 🧰 Tools & Resources

- **SIEM Platform:** Splunk (Free Edition)  
- **Log File:** `SOC_Task2_Sample_Logs.txt` (custom structured sample log)  
- **Tech Stack:** Splunk Web UI + SPL (Search Processing Language)

---

## 📋 Workflow Summary

### 1. Initial Setup

- Registered for a Splunk account and navigated to the dashboard.
- Uploaded the provided log data using the Splunk upload utility.
- Configured the inputs to cover Application, Security, and System logs.
- Validated data ingestion using a wildcard query which returned over **117K events**.

### 2. Query-Based Log Exploration

- Identified failed login attempts to highlight repeated access failures.
- Isolated successful logins to find potential compromised credentials.
- Used statistical aggregation to find users and IPs with abnormal login patterns.
- Cross-analyzed login and malware events to detect malicious activity.

### 3. Threat Correlation & Insights

- Mapped out users showing signs of brute-force login patterns.
- Flagged IP addresses linked to both login and malware entries.
- Investigated connections that might suggest lateral movement within the network.

### 4. Response Strategy

- 🔒 **Immediate Actions:** Flag and block suspicious IPs, reset passwords for impacted users, and isolate compromised endpoints.
- 🛡️ **Preventive Steps:** Enforce MFA, configure login rate limits, and set up real-time alerts for unusual activity.
- 🔁 **Routine Practices:** Ongoing monitoring of privileged accounts, refining detection logic, and improving staff awareness.

### 5. Reporting & Communication

- Drafted a mock incident report email with key findings for the SOC manager.
- Included summaries of affected IPs, users, and threat types with suggested next steps.

---

## 🎓 Key Takeaways

- Learned how to structure and execute effective SPL queries in Splunk.
- Understood the process of detecting and analyzing real-world attack patterns.
- Gained experience in correlating user behavior with system anomalies.
- Developed incident reporting and communication skills essential for SOC operations.

---

## 📢 Disclaimer

> All simulations were performed in a test lab using fake log data. No real systems or user information were accessed or harmed during this exercise.

---

## 👤 Author

**Sarita Sharma**  
Cybersecurity Intern – Future Interns Program  
📅 July 2025

---

## 🌐 Contact

For professional queries or collaboration, feel free to connect on [LinkedIn](https://www.linkedin.com/in/sarita-sharma).

