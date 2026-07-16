# Training Data Governance: A Pipeline Failure

*Companion post: Part 3 of the LinkedIn series*

> **Note:** This file is a structural skeleton reconstructed from the series outline. Drop in the exact published post text (and any visuals) to replace this placeholder — the framework mapping below stays valid either way.

## The Incident

An internal AI training data governance failure at a technology organization, framed not as a one-off data-quality slip but as a **pipeline governance failure** — a breakdown in the process controls that should have caught the issue before it reached the training pipeline, not just the specific data point that slipped through.

## Why "Pipeline Failure" Framing Matters

Treating this as a single bad data point invites a single fix. Treating it as a pipeline governance failure asks a harder, more useful question: *what upstream process should have caught this category of problem, and why didn't it?*

| Governance layer | Relevant framework |
|---|---|
| Data provenance & lineage | NIST AI RMF (Map), ISO/IEC 42001 |
| Risk categorization of training sources | MIT AI Risk Repository |
| Organizational accountability for pipeline sign-off | NIST AI RMF (Govern), ISO/IEC 42001 (management system controls) |

## Analysis

The framing deliberately avoids naming the organization involved, consistent with the series convention of generic references. The point isn't to single out one company's mistake — it's that training data governance is a *process* discipline, and process failures are structural, not incidental.

## Governance Questions

1. Who signs off on a training data source before it enters a pipeline — and is that sign-off documented anywhere an auditor could find it?
2. Does your organization have a data lineage record that could answer "where did this come from" after the fact, or only at ingestion time?
3. Is there a defined risk tier for training data sources, or is all data treated as equivalent once it's inside the pipeline?
4. If a governance gap like this were discovered today, is there a documented remediation path, or would the response be improvised?
