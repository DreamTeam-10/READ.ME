# AI Hallucination Defense: A Three-Layer Model

*Companion post: Part 2 of the LinkedIn series*

> **Note:** This file is a structural skeleton reconstructed from the series outline. Drop in the exact published post text (and any visuals) to replace this placeholder — the framework mapping below stays valid either way.

## The Problem

A "Policy Advisor" or decision-support agent is only as trustworthy as its ability to avoid confidently stating things that aren't true. Hallucination isn't a cosmetic bug in agentic systems — it's a trust and safety failure mode with the same blast radius as a misconfigured permission.

## The Three-Layer Defense Model

| Layer | What it does | Framework anchor |
|---|---|---|
| **1. Least Privilege** | Constrain what the model can assert authoritatively by limiting its access and action scope — reduce the surface area where a hallucination can cause downstream harm. | NIST AI RMF (Manage), OWASP Agentic Top 10 (excessive agency) |
| **2. Automated Verification** | Programmatic checks — retrieval grounding, output schema validation, cross-referencing against source-of-truth systems — catch unsupported claims before they reach a human. | MITRE ATLAS (AI Trust & Robustness layer), NIST AI RMF (Measure) |
| **3. Human Oversight** | A human-in-the-loop checkpoint for the subset of outputs that carry real consequence if wrong — the layer that catches what automated verification can't. | NIST AI RMF (Govern), OWASP Agentic Top 10 (human oversight controls) |

## Why All Three Layers Matter

Each layer alone is insufficient: least privilege limits *damage* but not *frequency*; automated verification catches *known* failure patterns but not novel ones; human oversight doesn't scale to every output. Together, they form a defense-in-depth model for a class of AI failure that can't be patched away entirely.

## Governance Questions

1. Does your organization's AI risk register treat hallucination as a distinct risk category, or fold it into generic "model quality" concerns?
2. What's the actual scope of actions your decision-support agents can take *before* a human reviews their output?
3. Do you have automated verification in place today, or is human review your only check?
4. If a hallucinated output already reached a downstream decision, is there a documented containment and correction path?
