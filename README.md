# Nessus Authenticated Vulnerability Scan Lab

## Project Overview

This project demonstrates the difference between unauthenticated and authenticated vulnerability scanning using Tenable Nessus.

The goal of this lab is to show how credentialed vulnerability scans provide deeper visibility into target systems by allowing Nessus to perform local checks for missing patches, insecure configurations, installed software, and system-level vulnerabilities.

This lab builds on the previous Asset Discovery & Network Enumeration project.

---

## Objective

Compare unauthenticated and authenticated Nessus scan results against a RHEL 10 lab target.

This project demonstrates:

- Nessus scan configuration
- RHEL 10 SSH credentialed scanning
- Vulnerability scan comparison
- Authentication validation
- Vulnerability management documentation
- Remediation planning

---

## Lab Environment

| System | Role | IP Address | Operating System |
|---|---|---|---|
| Kali Linux | Nessus Scanner | 10.10.10.5 | Kali Linux |
| RHEL 10 | Authenticated Linux Target | 10.10.10.7 | Red Hat Enterprise Linux 10 |
| Windows VM | Separate Windows Auth Test Target | 10.10.10.4 | Windows |

---

## Tools Used

| Tool | Purpose |
|---|---|
| Tenable Nessus | Vulnerability scanning |
| Kali Linux | Scanner host |
| RHEL 10 | SSH credentialed Linux scan target |
| SSH | Linux authenticated checks |
| Windows VM | Separate Windows authentication test target |
| Markdown | Documentation |
| GitHub | Portfolio publishing |

---

## Project Structure

```text
nessus-authenticated-scan-lab/
│
├── README.md
│
├── screenshots/
│   ├── 01-nessus-dashboard.png
│   ├── 02-windows-target-ip.png
│   ├── 03-linux-target-ip.png
│   ├── 04-unauthenticated-scan-config.png
│   ├── 05-unauthenticated-scan-results.png
│   ├── 06-windows-credential-config.png
│   ├── 07-linux-ssh-credential-config.png
│   ├── 08-authenticated-scan-config.png
│   ├── 09-authenticated-scan-results.png
│   ├── 10-credentialed-checks-yes.png
│   └── 11-comparison-summary.png
│
├── exports/
│   └── export-note.md
│
├── notes/
│   ├── methodology.md
│   ├── scan-comparison.md
│   ├── findings-summary.md
│   └── lessons-learned.md
│
└── remediation/
    ├── top-5-findings.md
    └── recommended-next-steps.md
