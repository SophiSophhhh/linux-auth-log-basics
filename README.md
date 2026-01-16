#Project 1: linux-auth-log-basics

## Project Overview
This project demonstrates SOC fundamentals by analyzing Linux authentication logs (`auth.log`) to detect suspicious login activity. The focus is on manual log review, identifying failed login attempts, tracing IP addresses, and understanding risk exposure.
Note: This project uses a simulated authentication log to practice log analysis techniques.

## Skills Practiced
- Linux directory navigation and file handling
- Reading and analyzing log files
- Using `grep` to find failed login attempts
- Understanding IP addresses and network exposure
- Basic assessment of suspicious activity

## Example Analysis
Repeated failed login attempts from the same IP could indicate a brute-force attack. A SOC analyst would:
- Count failed attempts to identify abnormal patterns
- Determine if the source IP is internal or external
- Check whether multiple usernames are targeted
- Escalate the incident or block malicious sources if needed

## Tools Used
- Ubuntu (WSL)
- Linux commands: `cat`, `grep`, `ss`

## Future Improvements
- Automate log parsing using Bash or Python
- Correlate multiple log sources
- Expand detection to higher-risk services (SSH, RDP)
- Timestamp-based analysis for pattern detection
