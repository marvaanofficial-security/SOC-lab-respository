# Privilege Escalation Detection
spl
index=* sudo
| stats count by user, host
| sort - count
## Purpose 
Tracks sudo command usage an potential privilege escalation activity.
