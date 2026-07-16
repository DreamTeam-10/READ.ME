# Methodology

How incidents and policy developments get turned into framework-mapped analysis in this repo.

## The entry point is always a real event

Every case study starts with something that actually happened — a disclosed incident, a policy change, a vendor advisory. The framework mapping is derived *from* the incident, not imposed on it generically. If a framework doesn't meaningfully apply to the specific facts of the case, it's left out rather than forced in.

## The framework stack is the lens, not the topic

The active framework stack (see [`framework-reference.md`](framework-reference.md)) provides the vocabulary and structure for analysis:

- **NIST AI RMF** functions (Govern / Map / Measure / Manage) frame *who owns what* and *when in the lifecycle* a control applies.
- **MITRE ATLAS / ATT&CK / D3FEND** frame *how* an attack or failure actually unfolds at a technical level, and what countermeasure category addresses it.
- **OWASP Top 10 for Agentic Applications** frames risk specific to agentic architectures (tool misuse, memory poisoning, excessive agency).
- **MITRE F3** frames what happens *after* compromise, when access converts into financial fraud.
- **ISO/IEC 42001** frames the management-system / certification angle for organizations formalizing AI governance.

## Scope discipline

Broader cybersecurity stories (not AI-specific) are included only when they can be meaningfully reframed through an AI security lens. This keeps the body of work coherent and defensible rather than a general cybersecurity blog with AI keywords sprinkled in.

## Closing pattern

Each case study closes with **concrete, actionable governance questions** a team could bring into their next risk review — not a forward-looking teaser or a call to "stay tuned." The goal is that someone could read a single case study and walk away with something to actually check on Monday morning.

## Audience

Written to be legible to both technical and non-technical audiences. Visuals and summaries are designed to stand on their own without requiring the full technical writeup for context.
