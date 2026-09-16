# LearnCyber Multi Source SOC Investigation

## Overview

SOC investigation into suspicious activity targeting multiple LearnCyber attack surfaces.

The investigation correlated Wazuh alerts, Linux SSH authentication logs, Cloudflare Security Events, and threat intelligence to determine whether the activity represented isolated attacks or broader reconnaissance.

## Key Findings

• Repeated failed SSH authentication attempts targeted the `root` account.

• No successful SSH authentication was identified in the reviewed evidence.

• Cloudflare blocked a request for `/wp-config.php-backup`.

• Investigated IP addresses shared infrastructure associated with `AS48090`.

• The evidence supports broader reconnaissance or multi vector malicious
  activity, with medium confidence.

## Tools Used

• Wazuh
• Linux authentication logs
• Cloudflare
• VirusTotal
• AbuseIPDB
• Shodan

## MITRE ATT&CK

The confirmed activity maps primarily to:

• T1110.001, Password Guessing

Additional techniques were considered where supported by the available telemetry.

See [`mitre-mapping.md`](mitre-mapping.md).

## Investigation Report

The complete investigation, evidence analysis, timeline, threat intelligence, correlation assessment, and recommendations are available in:

[`incident-report.pdf`](incident-report.pdf)

## Evidence

Supporting screenshots are available in the [`evidence/`](evidence/) directory.

## Remediation

Containment and security improvement recommendations are documented in:

[`remediation.md`](remediation.md)
