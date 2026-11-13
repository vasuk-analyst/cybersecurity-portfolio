# SOC Analyst Portfolio — Azure Honeypot & Microsoft Sentinel

Open `index.html` to view the responsive SOC case study. It documents Azure VM provisioning, AMA/DCR log collection, Log Analytics, KQL, Sentinel alert triage, findings, limitations, and safe deallocation.

## Publish with GitHub Pages

Upload these three files to the repository root: `index.html`, `README.md`, and `azure-vm-status.png`. Then open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.

## Evidence and interpretation

The screenshot is cropped to show the VM resource group and `Stopped (deallocated)` status. Account, subscription and network values are excluded. No Sentinel or KQL screenshots were available in the source files.

The investigation summary records 924 failed logon events (4625), two source IPs reviewed, Logon Type 3 in reviewed events, no matching 4624 in the queried window, and Sentinel case #1899. It does not claim confirmed compromise or confirmed RDP attribution. A missing 4624 in a queried window is not proof that no successful access occurred outside that query's time or collection scope.

