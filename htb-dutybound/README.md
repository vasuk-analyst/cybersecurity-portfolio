# HTB DutyBound Security Project

> **Authorized lab work:** This portfolio summary describes learning activities in the Hack The Box DutyBound lab. It intentionally contains no walkthrough, flags, or machine-specific solution details.

## Project overview

This project involved a structured security assessment of a Linux target in Hack The Box Labs. I practised a methodical workflow from initial service discovery through application assessment, host-level investigation, and technical reporting.

The aim here is to showcase the skills and defensive thinking developed during the project without disclosing a solution to active HTB content.

## My contribution

- Performed network and web application enumeration in the authorized lab.
- Investigated application behavior and server-side input handling.
- Practised Linux host enumeration and privilege-escalation analysis.
- Recorded evidence and considered remediation and SOC monitoring opportunities.

## Environment and tools

| Area | Details |
|---|---|
| Platform | Hack The Box Labs |
| Target | DutyBound — Linux, Medium |
| Testing system | Kali Linux in VirtualBox |
| Network access | HTB Machines VPN |
| Tools observed in use | Nmap 7.95, Gobuster 3.8, curl, sqlmap 1.9.11, OpenVPN, Netcat |

Tool versions are included where they were visible in the collected terminal evidence. Confirm versions against your own notes before publishing a final version.

## Skills practised

- Network and service enumeration
- Web application route and behavior analysis
- Structured-input validation assessment
- Linux host enumeration
- Evidence-based reporting and remediation writing
- Translating offensive-security observations into defensive monitoring ideas

## SOC / defensive perspective

For a SOC-oriented review, I considered general monitoring opportunities such as:

- anomalous application requests and repeated input-validation failures;
- unexpected child processes launched by application or database services;
- unusual process activity in a kiosk or restricted user session;
- sensitive file changes followed by privileged service activation;
- unexpected changes to service configuration or automation scripts.

These are **general detection hypotheses**, not deployed or validated SIEM rules. No Microsoft Sentinel testing is claimed for this project.

## Evidence

Add only sanitized, non-spoiler screenshots that you captured yourself. Suggested evidence:

- `screenshots/01-project-overview.png` — a non-spoiler project overview;
- `screenshots/02-tooling.png` — tools used, with host details and IP addresses hidden;
- `screenshots/03-soc-detection-map.png` — your own high-level defensive monitoring diagram;
- `screenshots/04-remediation-summary.png` — a non-spoiler remediation summary.

Do not publish flags, credentials, VPN profiles, cookies, session tokens, active-machine solutions, or private group-member information. The screenshots directory is intentionally not populated in this starter repository.

## Limitations and attribution

Before adding a technical walkthrough, first confirm on HTB that DutyBound is officially retired and that publication is allowed under the current platform rules. Until then, keep the detailed report and solution private. The public portfolio summary here avoids solution steps. Make sure every claim reflects your own saved evidence and personal contribution.

## Defensive themes

- Apply least privilege to application, database, and system services.
- Validate structured input on the server and avoid exposing internal parser details.
- Avoid unsafe shell execution and use strict parsers for administrative data.
- Protect sensitive files and isolate kiosk sessions.
- Monitor unexpected process launches and privileged service activity.

## References

- Hack The Box, “Platform Rules,” [HTB Help Center](https://help.hackthebox.com/en/articles/12325897-hack-the-box-platform-rules).
- Hack The Box, “Streaming / Writeups / Walkthrough Guidelines,” [HTB Help Center](https://help.hackthebox.com/en/articles/5188925-streaming-writeups-walkthrough-guidelines).
- Hack The Box, “Introduction to HTB Labs,” [HTB Help Center](https://help.hackthebox.com/en/articles/5185158-introduction-to-htb-labs).

---

This public-facing repository summary is for an authorized Hack The Box lab. Keep any full solution private until HTB marks the machine retired and public solution sharing is permitted. It contains no flags, credentials, VPN configuration, or claim of SOC alert deployment.

