# Blue Team Mapper v2.0

[![GitHub Pages](https://github.com/atraxsrc/BlueTeamMapper/actions/workflows/pages/pages-build-deployment/badge.svg)](https://atraxsrc.github.io/BlueTeamMapper/)

**Comprehensive visual reference & workflow mapper for blue team / defensive security operations.**

A single-page, interactive defender dashboard mapping the full blue team lifecycle:

- Visibility → Detection → Triage → Response → Hardening → Intel/Hunt → Recovery

Built as a static HTML/CSS site using the beautiful **Tokyo Night** color palette.

Live version:  
https://atraxsrc.github.io/BlueTeamMapper/

## Features

- Clean, cyberpunk-inspired UI using Tokyo Night theme
- Full MITRE ATT&CK-aligned defense lifecycle diagram (SVG)
- End-to-end workflow chains (phishing → ransomware → ADCS → credential attacks, etc.)
- Detailed sections covering:
  - SIEM & log management
  - EDR / endpoint detection
  - Detection engineering (SIGMA, YARA, behavioral analytics)
  - Incident response lifecycle & AD/cloud IR
  - Threat hunting methodology & techniques
  - Identity & access security
  - Network security controls
  - Hardening & vulnerability management
  - Threat intelligence & deception
  - Tool arsenal & key detection signatures
- Responsive design, monospace typography, semantic color highlighting

## Screenshots

(You can add 1–3 screenshots here later – e.g. the main diagram, a flow chain, a details card grid)

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
