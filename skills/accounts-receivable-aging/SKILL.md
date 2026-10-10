---
name: accounts-receivable-aging
description: Reconcile local customer receivables, invoices, credit notes, and receipts; produce aging analysis and a traceable follow-up list. Use for AR close, overdue balances, and collection prioritization.
---

# Accounts Receivable Aging

Use only files the user provides or explicitly authorizes. Never connect to a bank, ERP, email, or customer system unless separately requested and approved.

## Workflow

1. Inspect the files and identify reporting date, currency, customer key, invoice date, due date, open amount, credit notes, and receipt fields. Ask about ambiguous column mappings and sign conventions.
2. Preserve source files. Normalize dates, currency, customer names, and document identifiers in a working copy. Record every normalization rule.
3. Match receipts and credit notes to invoices using exact identifiers first. Use customer, amount, and date only as secondary evidence. Keep ambiguous or partial matches unresolved; never force a match.
4. Reconcile opening balance + invoices - credits - receipts to ending balance where source data permits. Show unmatched transactions and reconciliation differences.
5. Calculate aging as of the requested date using the agreed basis (invoice date or due date) and buckets supplied by the user. If no buckets are given, use current, 1-30, 31-60, 61-90, and over 90 days and label them as an analysis convention.
6. Prioritize follow-up using amount, days overdue, disputes, and known payment commitments. Do not infer customer intent or declare an amount uncollectible.

## Deliverables

- Summary by customer and aging bucket, with total tie-out.
- Invoice-level overdue and unmatched item list with source row references.
- Follow-up queue with reason, evidence, and missing information.
- Assumptions, exclusions, and reconciliation limitations.

Keep customer and bank details out of public logs and prompts. Require human review before collection communication or accounting write-off.
