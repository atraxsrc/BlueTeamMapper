# Blue Team Mapper v3.0

[![GitHub Pages](https://github.com/atraxsrc/BlueTeamMapper/actions/workflows/pages/pages-build-deployment/badge.svg)](https://atraxsrc.github.io/BlueTeamMapper/)   [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Tokyo Night Theme](https://img.shields.io/badge/theme-Tokyo%20Night-blueviolet)](https://github.com/enkia/tokyo-night-vscode-theme)

**Comprehensive visual reference & workflow mapper for blue team / defensive security operations.**

A single-page, interactive defender dashboard mapping the full blue team lifecycle:

- Visibility → Detection → Triage → Response → Hardening → Intel/Hunt → Recovery

Built as a static HTML/CSS/JS site using the beautiful **Tokyo Night** color palette.

**Live version:**  
https://atraxsrc.github.io/BlueTeamMapper/

**Companion project:**  
[Red Team Mapper](https://atraxsrc.github.io/RedTeamMapper/) — the offensive counterpart.

## Why This Exists
Red vs Blue is most effective when both sides speak the same language.  
This mapper flips the Red Team perspective into practical defensive controls, detection opportunities, hardening steps, and hunting queries — all in one clean visual reference.

## Features
- Sticky sidebar navigation (260px) with grouped phase categories and scroll-spy active states
- 7-phase defense lifecycle bar (Visibility → Detection → Triage → Response → Hardening → Hunt → Recovery)
- End-to-end workflow chains (phishing → detection → containment → recovery, ADCS abuse, credential attacks, ransomware, cloud identity, etc.)
- Callout boxes (danger/warn/info/success) for critical rules, caveats, and key hardening priorities
- Detailed sections covering:
  - Infrastructure & SIEM/Log Management (log pipeline, retention tiers, parsing)
  - Access Controls & Identity Protection (MFA hierarchy, PAM, Entra ID hardening)
  - Endpoint Protection (EDR/XDR tuning, exclusion hygiene, tamper protection)
  - Detection Engineering (Sigma rules, KQL queries, SPL hunt queries, YARA)
  - Technique Detection Matrix (22 techniques mapped to log source and event IDs)
  - SOAR Playbooks (phishing, lateral movement, ransomware, cloud identity)
  - Containment & Incident Response (isolation, evidence collection, chain of custody)
  - Threat Hunting Methodology (hypothesis-driven, IOC/TTP-based, behavioral)
  - Network & Data Protection (segmentation, DLP, proxy/TLS inspection)
  - Cloud & AD Hardening (ADCS ESC fixes, Entra ID CA policies, Tier 0 isolation)
  - MFA Strength Hierarchy with AitM bypass warnings
  - macOS/Linux Defense
  - AI Security Defense
  - Vulnerability SLA table (P0–P3 remediation timelines)
  - EDR blind spots (BYOVD, ETW tampering, syscalls, process ghosting, fork-and-run)
  - Full tool arsenal + critical Windows Event IDs & Sysmon references

## Screenshots
<img width="1871" height="1070" alt="image" src="https://github.com/user-attachments/assets/d3dfce3b-70f4-4ad5-8473-82ddb2365343" />
<img width="1871" height="1070" alt="image" src="https://github.com/user-attachments/assets/58cd18e2-6720-4337-97c1-196153bd6f6d" />
<img width="1871" height="1070" alt="image" src="https://github.com/user-attachments/assets/e61d8e9d-382a-43f2-bad7-89413e4e2a36" />

## Tech Stack

- HTML5 + CSS + JavaScript (vanilla, no frameworks)
- Google Fonts: **Syne** (headings) + **IBM Plex Sans** (body) + **JetBrains Mono** (code/mono)
- Extended Tokyo Night CSS variable system
- IntersectionObserver API for sidebar scroll-spy

## Tokyo Night Palette (Extended)

```css
:root {
  --bg:           #1a1b26;
  --bg-card:      #1e2030;
  --bg-raised:    #24283b;
  --bg-hover:     #292e42;
  --border:       #3b4261;
  --border-dim:   #2a2e42;
  --text:         #a9b1d6;
  --text-bright:  #cdd6f4;
  --text-dim:     #6c7086;
  --text-muted:   #45475a;
  --red:          #f7768e;
  --orange:       #e0af68;
  --yellow:       #e0af68;
  --green:        #9ece6a;
  --cyan:         #7dcfff;
  --blue:         #7aa2f7;
  --purple:       #bb9af7;
  --pink:         #bb9af7;
  --rose:         #f7768e;
  --teal:         #73daca;
}
```

## Changelog

### v3.0
- Added sticky sidebar navigation (260px) with grouped phase categories and IntersectionObserver scroll-spy
- Replaced SVG defense lifecycle diagram with clean 7-phase lifecycle bar
- Added Syne 800 as heading font; increased base font to 14px / line-height 1.75
- Added callout boxes (danger/warn/info/success) for critical rules and hardening priorities
- Extended CSS variable set with `--bg-card`, `--bg-raised`, `--bg-hover`, `--border-dim`, `--text-muted`
- Card accent bars (2px colored top-border per phase)
- New content: SOAR Playbooks, Splunk SPL hunt queries, Technique Detection Matrix (22 techniques), Vulnerability SLA table, ADCS ESC1/ESC4/ESC6 remediation, EDR blind spots, Evidence & Chain of Custody card, MFA Strength Hierarchy with AitM bypass warning

### v2.0
- Initial public release
