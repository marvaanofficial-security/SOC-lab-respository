# Brute Force Detection
'''spl
index=* "Failed password"
| stats count by src_ip 
| where count > 5

## Purpose
Detects multiple failed login attempts from the the same source ip
