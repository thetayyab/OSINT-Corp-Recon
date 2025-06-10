# OSINT-Corp-Recon
Corporate OSINT case study using open-source tools to identify digital exposure risks.

A practical walkthrough of corporate OSINT techniques used during an internship. This repo showcases real-world reconnaissance methods (with anonymized data) applied to assess digital exposure and weaknesses of an organization.

Project Scope
- Objective**: Identify potential weaknesses in a company's public-facing infrastructure using only open-source tools and intelligence.
- Focus Areas:
  - Subdomain Enumeration
  - Metadata Extraction
  - IAM Infrastructure Mapping
  - Technology Stack Fingerprinting
  - Public Service Misconfigurations

Repository Structure
```
OSINT-Corp-Recon/
├── README.md
├── reports/
│   ├── nas_summary.md
│   └── acme_corp_findings.md
├── screenshots/
│   ├── subdomain_scan.png
│   ├── plesk_panel_exposed.png
│   └── sso_misconfig.png
├── scripts/
│   ├── subdomain_enum.sh
│   └── metadata_extractor.py
└── tools_used.md
```

Tools & Techniques
- `Amass`, `Subfinder`, `crt.sh`, `dnsrecon`
- `ExifTool` for metadata leakage
- `Shodan`, `Censys` for exposed services
- `Dig`, `Whois`, `nslookup`, `theHarvester`

Sample Report Snippet
```
Title: Exposed Admin Panel on Subdomain
Severity: High
Details: The subdomain `admin.nas.com.au` was publicly accessible and exposed a Plesk login panel. No rate-limiting or MFA in place.
Recommendation: Restrict access to internal IPs and enforce MFA.
```

Disclaimer
All findings presented are fictionalized and sanitized for public demonstration. No real organization is exposed or harmed.

Contact
Created by: Tayyab Hameed; Cybersecurity Intern*  
For feedback or collaboration, connect via in/tayyabhameed1/ or open an issue.

---

> "Knowing your digital footprint is the first step in securing it."
