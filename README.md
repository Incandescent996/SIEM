# Correlation Rules
All the SIEM information.
Correlation rules play an important role in the timely detection of threats allowing analysts to take action on time. Correlation rules are pretty much logical expressions set to be triggered.

1. A User gets 5 failed Login Attempts in 10 seconds - Raise an alert for Multiple Failed Login Attempts
2. If login is successful after multiple failed login attempts - Raise an alert for Successful Login After multiple Login Attempts
3. A rule is set to alert every time a user plugs in a USB (Useful if USB is restricted as per the company policy)
4. If outbound traffic is > 25 MB - Raise an alert to potential Data exfiltration Attempt (Usually, it depends on the company policy)


Use Case 1 - If logs have been cleared or deleted
- The Log source is WinEventLog AND EventID is 104 - Trigger an alert **Event Log Cleared**
