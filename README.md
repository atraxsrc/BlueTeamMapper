# Blue Team Mapper v2.0

[![GitHub Pages](https://github.com/atraxsrc/BlueTeamMapper/actions/workflows/pages/pages-build-deployment/badge.svg)](https://atraxsrc.github.io/BlueTeamMapper/)   [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Tokyo Night Theme](https://img.shields.io/badge/theme-Tokyo%20Night-blueviolet)](https://github.com/enkia/tokyo-night-vscode-theme)

**Comprehensive visual reference & workflow mapper for blue team / defensive security operations.**

A single-page, interactive defender dashboard mapping the full blue team lifecycle:

- Visibility → Detection → Triage → Response → Hardening → Intel/Hunt → Recovery

Built as a static HTML/CSS site using the beautiful **Tokyo Night** color palette.

**Live version:**  
https://atraxsrc.github.io/BlueTeamMapper/

**Companion project:**  
[Red Team Mapper](https://atraxsrc.github.io/RedTeamMapper/) — the offensive counterpart.

## Why This Exists
Red vs Blue is most effective when both sides speak the same language.  
This mapper flips the Red Team perspective into practical defensive controls, detection opportunities, hardening steps, and hunting queries — all in one clean visual reference.

## Features
- Full MITRE ATT&CK-aligned defense lifecycle diagram (SVG)
- End-to-end workflow chains (phishing → detection → containment → recovery, ADCS abuse, credential attacks, ransomware, etc.)
- Detailed sections covering:
  - Infrastructure & SIEM/Log Management
  - Access Controls & Identity Protection
  - Endpoint Protection (EDR/XDR)
  - Detection Engineering (Sigma, KQL, SPL, YARA)
  - Containment & Incident Response
  - Threat Hunting Methodology
  - Network & Data Protection
  - Cloud & AD Hardening
  - macOS/Linux Defense
  - AI Security Defense
  - Full tool arsenal + critical Windows Event IDs & Sysmon references
- Responsive design with monospace typography and semantic color highlighting
- 100% static — loads instantly, no JS, no tracking

## Screenshots
<img width="1753" height="1357" alt="Screenshot_2026-03-03_21-39-38" src="https://github.com/user-attachments/assets/3278b2a5-9c6f-4001-a395-a2d7fbee72fd" />
<img width="1507" height="501" alt="Screenshot_2026-03-03_21-38-56" src="https://github.com/user-attachments/assets/2d6925eb-2cc0-443e-8b92-63bf44b22f6f" />


## Tech Stack

- HTML5 + CSS (custom variables)
- Google Fonts: JetBrains Mono + IBM Plex Sans
- Pure CSS variables based on **Tokyo Night** palette
- No JavaScript / frameworks — 100% static

## Tokyo Night Palette Used

```css
:root {
  --bg: #1a1b26;
  --bg-card: #24283b;
  --border: #414868;
  --text: #a9b1d6;
  --text-bright: #c0caf5;
  --text-dim: #565f89;
  --red: #f7768e;
  --orange: #e0af68;
  --yellow: #e0af68;
  --green: #9ece6a;
  --cyan: #7dcfff;
  --blue: #7aa2f7;
  --purple: #bb9af7;
  --pink: #bb9af7;
  --rose: #f7768e;
  --teal: #73daca;
}
