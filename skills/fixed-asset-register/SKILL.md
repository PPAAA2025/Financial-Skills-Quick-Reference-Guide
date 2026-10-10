---
name: fixed-asset-register
description: Reconcile a local fixed-asset register to ledger balances and movement records; recalculate depreciation using user-provided accounting policies and identify missing evidence.
---

# Fixed Asset Register Review

## Workflow

1. Confirm entity, period, currency, asset classes, capitalization threshold, depreciation method, useful lives, residual values, and depreciation start/stop conventions from the user's policy.
2. Preserve the original register. Normalize IDs and dates in a working copy; report duplicate IDs and missing fields.
3. Reconcile opening gross cost and accumulated depreciation plus additions, transfers, disposals, and depreciation to closing balances and the general ledger.
4. Recalculate period depreciation from the approved policy and supplied in-service/disposal dates. Do not assume a policy where the source is incomplete.
5. Identify assets with missing location/custodian, no movement, negative net book value, unexplained disposal, or inconsistent ledger mapping.
6. Present differences and evidence needed. Do not decide capitalization, useful life, impairment, or disposal accounting.

## Deliverables

- Register-to-ledger reconciliation.
- Asset-level depreciation recalculation and difference list.
- Additions/disposals and missing-evidence queue.
- Policy assumptions and unresolved accounting decisions.

All proposed adjustments require accountant review and approval before posting.
