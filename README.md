# Security Portfolio

Hands-on security projects focused on **Security Operations (SOC)**, investigation, and defensive thinking. This repository brings my project work together in one place.

## Featured projects

### SOC and detection

**[Azure Honeypot & Microsoft Sentinel](index.html)**  
End-to-end Azure lab covering Windows authentication telemetry, Azure Monitor Agent, Data Collection Rules, Log Analytics, KQL, Sentinel alert triage, and evidence-led case documentation.

- Reviewed 924 failed logon events (Event ID 4625) and examined two source IPs.
- Documented the limits of the investigation; no successful compromise or RDP activity is claimed.
- [View the case study](index.html)

### Security assessment labs

**[HTB DutyBound](htb-dutybound/README.md)**  
Authorized Hack The Box lab summary covering enumeration, web and host assessment, evidence handling, remediation themes, and general SOC monitoring hypotheses. No walkthrough, flags, or deployed SIEM detections are claimed.

## GRC

I have not added a GRC case study to this portfolio yet. As I complete GRC work, I will add it here with its scope, method, findings, and evidence clearly described. Possible future areas include risk assessment, control mapping, third-party risk, and business continuity.

## Repository layout

```text
soc-analyst-portfolio/
├── README.md
├── index.html                 # Azure honeypot and Sentinel case study
├── azure-vm-status.png        # Sanitized lab evidence
└── htb-dutybound/
    ├── README.md              # Non-spoiler project summary
    └── screenshots/           # Reserved for sanitized evidence
```

## How I present project work

Each project should explain its objective, my contribution, environment and tools, process, evidence, findings, limitations, and lessons learned. Only sanitized or synthetic data should be published. Never include credentials, personal data, private logs, or confidential organizational material.

## Contact

- GitHub: [@vasuk-analyst](https://github.com/vasuk-analyst)
