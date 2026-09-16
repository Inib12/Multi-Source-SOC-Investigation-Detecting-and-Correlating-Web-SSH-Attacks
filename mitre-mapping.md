## MITRE ATT&CK Mapping
### T1110.001, Password Guessing
#### Status: Confirmed
##### Evidence: 
Repeated SSH password authentication failures against the root account were observed in the Linux authentication logs.
This is the strongest MITRE ATT&CK mapping in the investigation.

### T1595, Active Scanning
#### Status: Potentially applicable
Threat intelligence associated 195.178.110.15 with scanning related activity, including port scanning.
However, threat intelligence classification alone does not prove that active scanning occurred against LearnCyber.
Therefore: T1595 is considered potentially applicable, but additional LearnCyber telemetry would be required to confirm active scanning against the organisation.

### T1190, Exploit Public Facing Application
#### Status: Potential, not confirmed
The Cloudflare event involved a request for: /wp-config.php-backup
The request was blocked by a Cloudflare rule associated with broken access control and file inclusion. However, requesting a potentially sensitive file does not by itself establish successful exploitation.
Therefore, T1190 is not presented as a confirmed technique.
