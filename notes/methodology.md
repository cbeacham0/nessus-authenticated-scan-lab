# Methodology

This lab followed a basic vulnerability management scanning workflow.

## Steps Performed

1. Verified the RHEL 10 target IP address.
2. Confirmed network connectivity from Kali/Nessus to the RHEL 10 target.
3. Prepared RHEL 10 for SSH-based credentialed scanning.
4. Created a dedicated RHEL 10 scan account named `nessus_scan`.
5. Added the RHEL 10 scan account to the `wheel` group for sudo access.
6. Verified SSH login from Kali to RHEL 10.
7. Ran an unauthenticated Nessus scan to establish a baseline.
8. Ran an authenticated Nessus scan using RHEL 10 SSH credentials.
9. Verified the authenticated scan displayed `Auth Pass`.
10. Compared unauthenticated vs authenticated scan visibility.
11. Documented key findings and recommended next steps.

## Scope

This project was performed in a controlled virtual lab environment.

Primary authenticated target:

- RHEL 10 Linux target at `10.10.10.7`

Additional troubleshooting target:

- Windows VM at `10.10.10.4`

No exploitation was performed. This lab focused on vulnerability discovery, credentialed scanning, and documentation.

## Tools Used

- Tenable Nessus
- Kali Linux
- RHEL 10
- SSH
- Windows VM
- Markdown
- GitHub

## Credential Handling

Credentials were configured directly inside the Nessus scan configuration.

Passwords were not documented, exported, or uploaded to GitHub.

Screenshots were captured only after hiding or avoiding sensitive password fields.

## Vulnerability Management Relevance

Authenticated scanning is a key part of vulnerability management because it provides deeper visibility into missing patches, insecure configurations, local software, and system-level exposures.
