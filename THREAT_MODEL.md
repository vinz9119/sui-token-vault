# Threat Model

### Assets
User-controlled assets deposited into the vault.

### Trust boundaries
- User
- Vault module
- Asset implementation
- Application/integration layer

### Threats
- Unauthorized withdrawal
- Accounting mismatch
- Incorrect asset-type handling
- Missing input validation
- Upgrade or admin privilege abuse

Before deployment, each invariant should have executable tests and the final package should be reviewed against the exact Sui framework version.
