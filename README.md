# Olamide Kamson — GRC Projects Portfolio

[![Live Portfolio](https://img.shields.io/badge/Live-Portfolio-0066cc?style=flat-square)](https://olamidekamson.github.io/grc-portfolio)
[![GRC](https://img.shields.io/badge/Domain-GRC%20%7C%20Risk%20%7C%20Compliance-gold?style=flat-square)]()
[![Location](https://img.shields.io/badge/Location-British%20Columbia%2C%20Canada-green?style=flat-square)]()

An interactive, single-file portfolio showcasing **10 Governance, Risk & Compliance projects** across four organisations — GTBank, Hope PSBank, Wema Bank, and Keff Tech Inc.

## Features

- **10 detailed project case studies** — each with challenge, deliverables, impact metrics, and real scenario Q&As
- **Filter by organisation** — view projects by GTBank, Hope PSBank, Wema Bank, or Keff Tech Inc
- **Modal deep-dives** — click any project card for the full case study with tabbed navigation
- **Experience timeline** — visual career arc with key achievements per role
- **Skills matrix** — frameworks, GRC domains, tools, and certifications
- **Interview scenario Q&As** — per project, showing how I'd handle real situations
- **Responsive** — works on desktop and mobile
- **Zero dependencies** — single HTML file, no build step required

## Projects Covered

| Organisation | Project | Domain |
|---|---|---|
| Keff Tech Inc | Enterprise Risk Register Development | Enterprise Risk |
| Keff Tech Inc | ISO 27001 / SOC 2 Audit Readiness | Audit & Compliance |
| Keff Tech Inc | PIPEDA / Bill C-27 Privacy Program | Canadian Privacy |
| Wema Bank | Third-Party Risk Management Program | TPRM |
| Wema Bank | NDPR Compliance Program | Data Protection |
| Wema Bank | Risk & Control Self-Assessment (RCSA) | Operational Risk |
| Hope PSBank | Digital Fraud Detection Controls | Fraud Risk |
| Hope PSBank | Risk-Aware KYC Onboarding Redesign | KYC / AML |
| GTBank | RBAC / IAM Governance Framework | Identity & Access |
| GTBank | DPIA Framework for New Products | Data Privacy |

## How to Deploy on GitHub Pages

1. **Fork or clone** this repository
2. Go to **Settings → Pages**
3. Set Source to `main` branch, root folder `/`
4. Your portfolio will be live at `https://yourusername.github.io/grc-portfolio`

## Local Preview

No build step needed — just open `index.html` in any browser:

```bash
# Option 1: Direct open
open index.html

# Option 2: Simple local server (Python)
python3 -m http.server 8000
# Then visit http://localhost:8000

# Option 3: VS Code Live Server extension
# Right-click index.html → Open with Live Server
```

## Customisation

All project data is in the `PROJECTS` object in the `<script>` section of `index.html`. Each project has:

```javascript
'project-id': {
  org: 'keff',          // keff | wema | hope | gtb
  icon: 'fa-solid ...',  // Font Awesome icon class
  title: '...',
  meta: ['Role', 'Frameworks', 'Period'],
  overview: '...',       // HTML string
  delivered: '...',      // HTML string
  impact: '...',         // HTML string
  scenarios: [
    { trigger: '...', q: '...', a: '...' }
  ]
}
```

To add a new project, add a new card in the `#card-grid` div and a matching entry in `PROJECTS`.

## Contact

- LinkedIn: [linkedin.com/in/olamidekamson](https://linkedin.com/in/olamidekamson)
- Location: British Columbia, Canada
- Open to: GRC, Data Protection, Risk, and Compliance roles across Canada

---

*Built as a single-file, zero-dependency portfolio for GitHub Pages deployment.*
