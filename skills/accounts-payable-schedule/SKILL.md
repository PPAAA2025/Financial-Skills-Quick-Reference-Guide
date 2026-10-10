---
name: accounts-payable-schedule
description: Reconcile local supplier statements, invoices, contract terms, approvals, and payment records into a due-date schedule and exception list. Use for AP aging and proposed payment planning.
---

# Accounts Payable Schedule

Create a review schedule only. Never initiate, approve, or submit a payment.

## Workflow

1. Identify the as-of date, planning horizon, currency, supplier/document keys, invoice and due dates, amount due, payment status, approval status, and source files.
2. Check duplicate invoice numbers, repeated amounts, supplier name variations, credit notes, partial payments, and date or currency inconsistencies.
3. Match payments to invoices by document reference first. Treat amount/date/name matches as candidates and retain uncertain matches for review.
4. Reconcile invoice balances to supplier statements or AP ledger when both are supplied. Show unmatched entries and explain the limitation when sources do not tie.
5. Group items by overdue, due within the planning horizon, and later. A proposed batch may consider due date, contractual terms, approval status, disputes, and user-provided cash constraints.
6. Do not invent payment priority or discount economics. Mark missing approvals, missing tax invoices, disputes, and bank-detail changes as blockers for human review.

## Deliverables

- Invoice-level due schedule with source references.
- Proposed payment batches clearly labeled as recommendations, not approvals.
- Exception list: duplicates, missing documents, mismatches, disputes, and overdue items.
- Tie-out, assumptions, and unresolved items.

Do not include full bank account details in ordinary reports. Any change to supplier payment instructions requires independent verification outside this workflow.
