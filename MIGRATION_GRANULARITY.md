# Migration Granularity Notes

- Repository: `fintechbankx-payments-initiation-settlement-service`
- Source monorepo: `enterprise-loan-management-system`
- Sync date: `2026-03-15`
- Sync branch: `chore/granular-source-sync-20260313`

## Applied Rules

- dir: `payment-context` -> `.`
- dir: `payment-service` -> `legacy/payment-service`
- file: `api/openapi/payment-context.yaml` -> `api/openapi/payment-context.yaml`
- dir: `infra/terraform/services/payment-initiation-service` -> `infra/terraform/payment-initiation-service`
- file: `docs/architecture/open-finance/capabilities/hld/payment-initiation-service-hld.md` -> `docs/hld/payment-initiation-service-hld.md`
- file: `docs/architecture/open-finance/capabilities/test-suites/payments-test-suite.md` -> `docs/test-suites/payments-test-suite.md`

## Notes

- This is an extraction seed for bounded-context split migration.
- Follow-up refactoring may be needed to remove residual cross-context coupling.
- Build artifacts and local machine files are excluded by policy.

