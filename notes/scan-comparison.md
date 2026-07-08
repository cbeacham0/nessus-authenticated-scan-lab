# Scan Comparison

## Purpose

This document compares unauthenticated and authenticated Nessus scan results for the RHEL 10 target.

The unauthenticated scan observed the system externally without logging in. The authenticated scan used SSH credentials with sudo privilege escalation to perform deeper local checks.

---

## Target

| Target | System | Authentication Method |
|---|---|---|
| 10.10.10.7 | RHEL 10 | SSH credentials with sudo |

---

## Results Summary

| Scan Type | Critical | High | Medium | Low | Info | Authentication |
|---|---:|---:|---:|---:|---:|---|
| Unauthenticated | TBD | TBD | TBD | TBD | TBD | No credentials used |
| Authenticated | TBD | TBD | TBD | TBD | TBD | Auth Pass |

---

## Evidence Note

PDF and CSV scan exports were not included because the Nessus version used in this lab did not support report exporting.

Scan evidence was captured through screenshots and documented findings.

---

## Windows Authentication Note

A separate Windows authenticated test scan was created for the Windows target at `10.10.10.4`.

The Windows host was reachable, but Windows authentication required additional troubleshooting. To keep the lab focused and accurate, the successful authenticated scan evidence in this project is based on the RHEL 10 target at `10.10.10.7`.

No Windows credentials or passwords are stored in this repository.

---

## Key Differences Observed

| Area | Unauthenticated Scan | Authenticated Scan |
|---|---|---|
| Patch visibility | Limited | Improved |
| Local configuration checks | Limited | Improved |
| Installed software detection | Limited | Improved |
| Missing updates | Limited | Improved |
| Risk accuracy | Lower | Higher |

---

## Analysis

The authenticated scan provided better visibility because Nessus was able to log into the RHEL 10 target using SSH and perform local security checks.

This reduced reliance on network-only detection and provided more actionable vulnerability information for remediation planning.

---

## Conclusion

Authenticated vulnerability scanning is useful for enterprise vulnerability management because it provides deeper system-level visibility and supports more accurate remediation planning.
