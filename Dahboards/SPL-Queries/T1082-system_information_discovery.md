# Technique: System Information Discovery
spl
index=* ("uname" OR "hostname" OR "whoami")
| stats count by user

T1082-System Information Discovery
