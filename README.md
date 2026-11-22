# Home-Lab SOC with Wazuh: Detection Engineering & Automated Response

## Project Overview
This repository contains the literature review, configuration artifacts, custom detection rules, and automated response scripts for a bachelor's thesis on building a reproducible, open-source Security Operations Center (SOC) in a home-lab environment.

Using **Wazuh** as the SIEM/HIDS platform and **Sysmon** on a monitored Windows endpoint, this project evaluates out-of-the-box detection coverage against simulated **MITRE ATT&CK** techniques executed via **Atomic Red Team**. For techniques that bypass default rules, custom XML decoders/rules and time-limited active response scripts (e.g., temporary IP blocking) are engineered and re-tested. The system is evaluated before and after customization based on detection coverage, false-positive rate, and lab reproducibility.

## Repository Structure
```text
.
├── README.md
└── literature/
    ├── pdfs/                  # Full-text PDF copies of all 16 reviewed sources
    ├── notes/                 # Reading notes mapping each source to thesis sections
    └── references.bib         # Complete BibTeX bibliography
```

## Literature Overview

| # | BibTeX Key | Topic / Focus | Thesis Relevance |
| :--- | :--- | :--- | :--- |
| 1 | `gonzalez2021siem` | SIEM architecture, trends, and open-source vs. commercial tools | Background / State of the Art |
| 2 | `chamkar2025wazuh` | Threat detection, false positives, and performance in Wazuh | Problem Statement & Evaluation |
| 3 | `teixeira2019ossec` | OSSEC/Wazuh internals, Active Response, and false-block risks | System Architecture & Active Response |
| 4 | `alboushy2026smartsiem` | Context-aware multi-step detection and MITRE mapping in Wazuh | Related Work & Custom Rule Design |
| 5 | `strom2020attack` | MITRE ATT&CK design, structure, and philosophy | Theoretical Foundation |
| 6 | `strom2017finding` | Threat-based behavioral analytics and adversary emulation | Core Methodology |
| 7 | `chamkar2024soc` | SOC use case lifecycle and ATT&CK coverage gap analysis | Core Methodology (Gap Analysis) |
| 8 | `lupinacci2026trace2attack` | Reproducible telemetry generation with Atomic Red Team | Experimental Setup & Reproducibility |
| 9 | `kent2006nist80092` | NIST SP 800-92 guide to security log management | Background / Log Pipeline Standards |
| 10 | `mavroeidis2018sysmon` | Windows endpoint visibility and threat hunting using Sysmon | Telemetry Selection |
| 11 | `thomas2022hespids` | Sysmon filtering and Atomic Red Team testing (T1055) | Implementation & False-Positive Control |
| 12 | `shukla2025rulegenie` | SIEM rule optimization, precision, recall, and false alarms | Detection Engineering & Metrics |
| 13 | `nelson2025nist80061r3` | NIST SP 800-61 Rev. 3 incident response & containment | Incident Response Framework |
| 14 | `alahmadi2022falsepositives` | Empirical study on SOC alert fatigue and false positives | Motivation & Evaluation Discussion |
| 15 | `kremer2023icsecure` | Automated incident response playbooks and SOAR workflows | Automated Response & Future Work |
| 16 | `ukwandu2020cyberranges` | Survey of virtualized cyber ranges and security testbeds | Lab Design & Reproducibility |
