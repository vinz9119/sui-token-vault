# Accounting Model

For each supported asset, the vault maintains an internal balance for each owner.

The core invariant is:

**recorded balances must equal the assets actually controlled by the vault**, subject to any explicitly documented rounding or fee policy.

Every state-changing operation should make its preconditions and postconditions testable.

## Review questions
- Can an unauthorized caller change another owner's balance?
- Can a withdrawal exceed the recorded balance?
- Are zero-value operations rejected?
- Is every asset type handled consistently?
