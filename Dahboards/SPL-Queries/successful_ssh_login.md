# Successful SSH login Detection
spl
index=* "Accepted password"
| rex "Accepted password for (?<user>\w+)"
| stats count by user 
| sort - count
## Purpose 
Detects successful SSH logins and identifies the most active users.
