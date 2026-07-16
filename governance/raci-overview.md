# AI Agent Governance RACI — Overview

[View the matrix](AI_Governance_RACI_v01.csv)

## What this is

A control-level RACI matrix for agentic AI deployments, mapping 16 controls across identity, memory security, prompt injection, zero trust access, and emergency shutdown to nine organizational roles. It's built to answer a question most AI governance decks skip: *when something goes wrong with an agent, who is actually accountable, and who just needs to be told?*

## How it's structured

**Rows** are organized under the four **NIST AI RMF** functions:
- **GOVERN** — identity registration, agent inventory, human-in-the-loop (HITL) escalation policy, tool registry governance, zero trust architecture
- **MAP** — memory attack surface, agent-to-agent trust boundaries, prompt injection exposure, tool permission blast radius, action reversibility
- **MEASURE** — anomaly detection, memory poisoning checks, HITL bypass metrics, supply chain monitoring, audit trail completeness
- **MANAGE** — kill switch / emergency shutdown, incident response playbooks, least-privilege remediation, lifecycle decommissioning

Each control also carries an **OWASP Agentic Top 10** reference (`ASI01`–`ASI10`) and, where relevant, a legacy **LLM Top 10** reference (`LLM01`), so the matrix reads consistently whether you're coming at it from an AI risk background or an application security background.

**Columns** carry standard RACI assignments (Responsible / Accountable / Consulted / Informed) across nine roles: CISO / AI Risk, AI Governance Board, Product/App Team, Security Engineering, MLOps/Platform, Legal & Compliance, Data Governance, IT Ops/Infra, and Business Unit Owner.

## Template fields, intentionally unpopulated

Two columns — **ZTA Check IDs** and **ZTA Status/Date** — are left as a template scaffold rather than filled with placeholder data. They're designed to link to an organization's own Zero Trust Architecture assessment tracking, so the matrix can go from reference document to active tracker without restructuring.

## How to use it

1. Start with **Risk Level** (Critical/High) to prioritize which controls get assigned owners first.
2. Confirm the RACI assignment matches your actual org chart — the roles here are a common-denominator starting point, not a prescription.
3. Populate ZTA Check IDs once your organization has a corresponding assessment framework in place.
4. Revisit quarterly — several controls (tool permission review, credential rotation posture) are explicitly designed as recurring checks, not one-time setup.

## Framework alignment

| Layer | Maps to |
|---|---|
| Row structure | NIST AI RMF (Govern / Map / Measure / Manage) |
| Risk references | OWASP Top 10 for Agentic Applications (ASI01–10), legacy LLM Top 10 (LLM01) |
| Underlying threat model | MITRE ATLAS (prompt injection, memory poisoning), MITRE ATT&CK (supply chain, credential access) |
