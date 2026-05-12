Rule Name

Repeated Failed Login Attempts

Description

Detects multiple failed login attempts from the same IP address or against the same user within a short timeframe. This may indicate password spraying, brute-force activity, or unauthorized access attempts.

That description is long enough for Sentinel and sounds professional for interviews.

For the rest of the fields:

MITRE ATT&CK Tactic: Credential Access
Technique: Brute Force (T1110)
Severity: Medium or High
Status: Enabled

For the KQL query, if you are using Entra ID sign-in logs, a common beginner-friendly version is:

<img width="1547" height="797" alt="image" src="https://github.com/user-attachments/assets/13a11125-8b3d-4829-b8fe-de303b084b48" />


What this does:

Looks for failed sign-ins
Groups them into 5-minute windows
Alerts if there are 5 or more failures

<img width="1603" height="861" alt="image" src="https://github.com/user-attachments/assets/0bfd912c-0f9c-4535-b357-a1c8a915b300" />

