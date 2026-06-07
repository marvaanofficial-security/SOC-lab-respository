# Failed Login Detection 
'''spl 
index=* "Failed passwd"
| stats count by user
| sort - count
## Purpose
Shows accounts with the highest number of failed login atempts.
