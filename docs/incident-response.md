# Incident Response Playbook

## Objective

Document the investigation of suspicious SSH authentication activity on the authorized Azure lab virtual machine.

## Detection

Identify repeated failed SSH authentication attempts using Linux Syslog events in Log Analytics.

## Investigation Steps

1. Review the event timestamps.
2. Identify the affected virtual machine.
3. Examine available source IP and username information.
4. Check whether any successful authentication followed the failed attempts.
5. Review relevant Azure administrative activity where appropriate.

## Response

- Validate whether the activity was generated during authorized testing.
- Restrict SSH access to trusted source IP addresses.
- Review SSH authentication settings.
- Rotate credentials if exposure is suspected.
- Record remediation and verify the result.

## Evidence

Add sanitized query results and screenshots after the lab has been implemented and tested.

## Status

Playbook prepared. No incident detection or remediation is claimed until verified in the lab.
