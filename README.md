# Incident Response Analysis Project

## Overview

This project simulates a security incident involving repeated failed login attempts from a suspicious IP address.

The goal is to detect, analyze, and respond to potential brute-force attack behavior using basic security tools.


## Scenario

Multiple failed login attempts were detected from a single IP address (10.0.0.50).

This activity may indicate a brute-force attack attempting to gain unauthorized access.


## Detection (SQL Analysis)

SQL queries were used to analyze login data and identify suspicious activity.

A specific IP address (10.0.0.50) showed a significantly high number of failed login attempts compared to others.

### SQL Result
<img width="1040" height="434" alt="sql-detection-result" src="https://github.com/user-attachments/assets/d177dc61-5c78-453c-8956-3ef56f637cbe" />

## Analysis

### Log Analysis (SQL)

* Identified repeated failed login attempts
* Grouped activity by IP address
* Detected abnormal login patterns

### Network Analysis (Wireshark)

Wireshark was used to capture and analyze normal network traffic from a local machine to understand baseline behavior.

Although the exact attack traffic was not captured, this analysis helps establish a reference for identifying abnormal patterns such as repeated or automated requests.

### Wireshark Capture
<img width="1439" height="900" alt="dns-analysis" src="https://github.com/user-attachments/assets/6aa56dcf-bd02-4724-bbd4-38a5886f85bb" />


## Findings

* Suspicious IP: 10.0.0.50
* Pattern: Multiple failed login attempts
* Possible Threat: Brute-force attack


## Response

Based on the identified suspicious activity, the following response actions are recommended:

* Block the suspicious IP address
* Monitor for further unusual activity
* Implement account lockout policies
* Enable alerting for repeated login failures

These actions are proposed as part of a simulated incident response process.

## Key Takeaways

* SQL can effectively detect suspicious login behavior
* Understanding normal network traffic is essential for identifying anomalies
* Basic tools can be used to simulate real-world security analysis


## Conclusion

This project demonstrates how security incidents can be detected using log analysis and better understood through network traffic analysis.

It highlights the importance of combining multiple tools to identify and respond to potential threats.
