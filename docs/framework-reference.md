# AI Security & Governance — Framework Reference

Consolidated reference for cross-framework AI security work (agentic AI security, governance, and skills-mapping projects) used throughout this repo, RACI documentation, and companion reports.

## Core Framework Matrix

| Framework | Current Version | Operational Scope | Canonical Docs |
|---|---|---|---|
| 🛡️ MITRE ATT&CK | v19.1 | Adversary tactics, techniques, and procedures (TTPs) targeting traditional enterprise networks. 15 Enterprise tactics · 286 techniques. | attack.mitre.org |
| 🏦 NIST CSF | 2.0 | High-level guidance for managing, prioritizing, and reducing systemic organizational cybersecurity risk. 6 functions · 22 categories. | nist.gov/cyberframework |
| 🤖 MITRE ATLAS | v5.4 | Adversarial threat landscape targeting AI/ML systems (prompt injection, data poisoning, etc.). 16 tactics · 84 techniques. | atlas.mitre.org |
| 🧱 MITRE D3FEND | v1.3 | Technical knowledge base of engineering countermeasures to detect, isolate, and deceive adversaries. 7 categories · 267 techniques. | d3fend.mitre.org |
| 🧠 NIST AI RMF | 1.0 | Risk management guidance for trustworthy/secure AI governance (Govern, Map, Measure, Manage). 4 functions · 72 subcategories. | nist.gov/ai-rmf |
| 💸 MITRE F3 (Fight Fraud Framework) | v1.1 (released 2026-04-09) | Post-compromise behaviors — how access converts into financial fraud, via Positioning and Monetization. 8 tactics · 123 techniques. | ctid.mitre.org/fraud |
| 📋 OWASP Top 10 for Agentic Applications | 2025 | Top risks specific to agentic AI application design and deployment. | owasp.org/Top10/2025 |
| 🎓 MIT AI Risk Repository | — | Living taxonomy/database of AI risks for prioritization work. | airisk.mit.edu |

**Watch item:** ISO/IEC 42001 (AI management systems) — the applicable reference for AI governance/management system certification is **ISO/IEC 42001:2023**.

## Operational Scopes Explained

**🌐 Infrastructure Defense Layer** (ATT&CK / D3FEND)
Blocking unauthorized system access and cataloging countermeasures to break the enterprise attack lifecycle.

**🛡️ AI Trust & Robustness Layer** (ATLAS / AI RMF)
Programmatic boundaries — output schema constraints, validation firewalls — to defend agentic systems against runtime prompt injection and adversarial ML threats.

**💸 Financial Fraud Layer** (MITRE F3)
Bridges technical compromise and monetization. Adds two tactics ATT&CK doesn't enumerate:
- **Positioning (FA0001)** — post-access prep: synthetic-identity seeding, account warming, beneficiary setup, SIM-swap pre-positioning, banking-session hijack.
- **Monetization (FA0002)** — converting stolen assets to funds: money-mule layering, authorized-push-payment (APP) fraud, crypto off-ramping, card cash-out, refund/chargeback abuse.

Fraud-specific techniques use `F1XXX` IDs (e.g. F1005.003 Add Beneficiary, F1025.003 Wire Transfer); reused ATT&CK techniques keep `T1XXX` IDs.

**📋 Agentic Application Layer** (OWASP Top 10 for Agentic Apps)
Risks specific to how agentic systems are architected and deployed (tool misuse, excessive agency, memory poisoning, etc.).

## Related Research Threads

- **TRAIT&R** (Taxonomy of Rogue AI Tactics and Routines) — an ATT&CK-style TTP framework adapted for hypothetical misaligned/insider AI adversaries, built on MITRE ATT&CK's tactic/technique structure.
- **agentskills.io** open standard — used as the skill-authoring format in cross-framework skill libraries.

## Version Tracking Note

Version numbers (ATT&CK v19.1, ATLAS v5.4, D3FEND v1.3, F3 v1.1) should be spot-checked periodically against source sites, as MITRE and NIST update these on independent cycles.

*Last compiled: July 2026.*
