---
name: cash-flow-forecast
description: Build a short-term rolling cash forecast from user-provided opening balances, receipts, payments, payroll, taxes, and other cash flows. Use for liquidity planning and cash-gap scenarios without connecting to bank feeds.
---

# Cash Flow Forecast

## Workflow

1. Confirm forecast horizon, time buckets, currencies, legal entities, and whether the user wants direct cash receipts/payments or an indirect method.
2. Identify opening available cash and restricted balances separately. Verify the as-of date and reconcile opening cash to supplied bank or ledger totals where possible.
3. List forecast inflows and outflows by date, amount, currency, category, source, and confidence. Separate contracted/approved items from estimates and uncommitted opportunities.
4. Avoid double counting invoices, tax payments, payroll, transfers between accounts, and items already reflected in opening cash.
5. Calculate opening cash + inflows - outflows = closing cash for every bucket. Flag negative or below-threshold balances against a threshold supplied by the user.
6. Prepare a base case and clearly labeled sensitivity cases, such as delayed receipts or accelerated supplier payments. Change only assumptions the user approves or explicitly asks to test.
7. Identify the date and drivers of any projected shortfall. Do not recommend borrowing, investment, or payment actions as if approved.

## Deliverables

- Period-by-period cash bridge with source references.
- Assumption register with amount, date, status, and confidence.
- Base and sensitivity case comparison.
- Data gaps and decisions requiring management confirmation.

Keep currencies separate unless an exchange rate and conversion date are provided. Never use forecast output to initiate transfers or payments.
