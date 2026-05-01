This project documents a comprehensive Digital Forensics & Incident Response (DFIR) investigation performed on a compromised enterprise workstation using the M57 “Jean” dataset from Digital Corpora.

The investigation focused on identifying indicators of compromise (IOCs), analyzing attacker behavior, and reconstructing the full incident timeline. The findings indicate a confirmed security breach involving unauthorized access, suspicious system activity, and potential data exfiltration.

 Objectives
Ensure forensic integrity of acquired evidence
Perform in-depth disk and artifact analysis
Identify malicious or unauthorized activities
Reconstruct the attack lifecycle
Assess potential data exfiltration paths
Map observed behavior to established threat frameworks
Tools & Technologies
Autopsy — Digital forensic analysis & artifact extraction
FTK Imager — Evidence acquisition and hash verification
Velociraptor — Endpoint visibility and threat hunting
EnCase — Advanced forensic processing
Methodology
1. Evidence Acquisition & Validation
Forensic image integrity verified using cryptographic hash values (MD5/SHA1)
Chain of custody principles maintained throughout the process
2. Disk & File System Analysis
Disk image examined using Autopsy
Identification of user activity, file access patterns, and installed applications
3. Artifact Analysis

Key forensic artifacts were analyzed, including:

Windows Registry → user accounts, persistence mechanisms
Prefetch Files → execution history of applications
Email Data (PST Files) → communication and exfiltration evidence
Web Artifacts → browsing history and deleted records
4. Threat Hunting & Behavioral Analysis
Velociraptor used to simulate proactive threat hunting
Suspicious patterns and anomalies identified across system activity
 Key Findings
Indicators of Compromise (IOCs)
Unauthorized user account creation
External device connections (USB/mobile)
Evidence of remote system access
Installation of unapproved software
Evidence of Malicious Activity
Access to sensitive and confidential files
Email-based data exfiltration identified via PST analysis
Deleted browser artifacts suggesting anti-forensic techniques
 Incident Assessment

The investigation indicates:

A confirmed compromise of the system
Multiple potential attack vectors
Behavioral patterns consistent with both insider activity and external intrusion

Notably, the presence of anti-forensic actions (artifact deletion) suggests an attempt to evade detection and complicate attribution.
