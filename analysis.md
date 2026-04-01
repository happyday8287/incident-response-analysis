## Analysis

Using SQL queries, failed login attempts were analyzed and grouped by IP address.

The IP address 10.0.0.50 showed a significantly higher number of failed login attempts compared to others.

Further investigation revealed repeated login attempts within a short time period, which is consistent with brute-force attack behavior.

## Tools Used

* SQL (log analysis)
* Wireshark (network traffic analysis)

## Findings

* Suspicious IP: 10.0.0.50
* Pattern: Multiple failed login attempts
* Risk: Potential unauthorized access attempt
