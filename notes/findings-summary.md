# Findings Summary

## Overview

This lab compared unauthenticated and authenticated Nessus vulnerability scans against a RHEL 10 lab target.

The authenticated scan provided deeper visibility by using valid SSH credentials with sudo access to perform local checks.

---

## Target Systems

| IP Address | Host Type | Role | Scan Type |
|---|---|---|---|
| 10.10.10.7 | RHEL 10 | Linux Target | Unauthenticated and authenticated |
| 10.10.10.4 | Windows | Separate test target | Windows authentication troubleshooting |

---

## Unauthenticated Scan Summary

| Severity | Count |
|---|---:|
| Critical | TBD |
| High | TBD |
| Medium | TBD |
| Low | TBD |
| Info | TBD |

---

## Authenticated Scan Summary

| Severity | Count |
|---|---:|
| Critical | TBD |
| High | TBD |
| Medium | TBD |
| Low | TBD |
| Info | TBD |

---

## Top Findings

| Finding | Severity | Affected Host | Remediation Summary |
|---|---|---|---|
| TBD | TBD | 10.10.10.7 | TBD |
| TBD | TBD | 10.10.10.7 | TBD |
| TBD | TBD | 10.10.10.7 | TBD |
| TBD | TBD | 10.10.10.7 | TBD |
| TBD | TBD | 10.10.10.7 | TBD |

---

## Key Observation

The authenticated scan produced improved visibility because Nessus successfully authenticated to the RHEL 10 target using SSH credentials.

## Windows Authentication Note

A Windows authenticated scan was tested separately for `10.10.10.4`. Authentication required additional troubleshooting and was separated from the successful RHEL 10 credentialed scan workflow.

## Recommended Next Steps

1. Prioritize critical and high findings.
2. Validate whether findings apply to the RHEL 10 target.
3. Create remediation tickets.
4. Patch or harden affected services.
5. Rescan to confirm remediation.
6. Continue troubleshooting Windows authenticated scanning as a follow-up task.
