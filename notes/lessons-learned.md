# Lessons Learned

This lab demonstrated the difference between unauthenticated and authenticated vulnerability scanning.

## Key Lessons

- Unauthenticated scans provide an external view of the target.
- Authenticated scans provide deeper system-level visibility.
- Credentialed checks help identify missing patches and local configuration issues.
- RHEL 10 authenticated scanning requires SSH access and sudo privilege escalation.
- Incorrect credentials can cause authentication failures or incomplete scan results.
- Windows authenticated scanning requires correct credentials, local administrator rights, SMB access, WMI firewall rules, and Remote Registry.
- Nessus scan screenshots and Markdown notes can still provide strong evidence when exports are not available.
- Comparing scans helps explain the business value of credentialed scanning.

## Professional Relevance

This project simulates a common enterprise vulnerability management workflow. In real environments, vulnerability teams use authenticated scans to improve scan accuracy, reduce blind spots, and support remediation planning.

## Next Lab

The next project will focus on CVE triage and risk-based prioritization using Nessus scan results.
