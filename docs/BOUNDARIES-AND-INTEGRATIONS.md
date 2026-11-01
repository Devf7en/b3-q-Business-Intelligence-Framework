# Boundaries and Integrations

## Domain ownership
- **BI Framework:** semantic models, metric definitions, analytical products, dashboards/reporting contracts, analytics and decision-support lifecycle.
- **b3Ɛq Core:** current shared runtime and existing BI/ETL module host; common IAM, tenant, audit, notification and integration capabilities.
- **ETL (Core module 104450):** existing pipeline metadata and orchestration model; do not duplicate its registry without an approved replacement plan.
- **Operational verticals:** own transactional records (Finance, SCM, TMS, CRM, HR, MES, WMS, etc.).
- **DataOS / Nigeria DataOS:** domain data stewardship, canonical entities and jurisdictional data products.
- **KMS:** knowledge assets and knowledge governance.
- **Ethos Intelligence:** enterprise ethos/intent interpretation, not metric storage.
- **Enterprise Observability:** telemetry/health signals; BI may consume governed operational measures but should not replace platform observability.
- **Enterprise Communications:** notification and communication delivery services.

## Integration patterns
- Versioned REST/event/data-product contracts.
- Explicit tenant and authorization context.
- Idempotent ingestion with replay and checkpoint semantics.
- Schema evolution and compatibility policy.
- Provenance, lineage and quality evidence.
- No direct database coupling unless explicitly approved and documented.

## Contract ownership
The source domain owns source schema and event semantics. BI owns analytical transformation contracts and metric semantics. Shared identity, tenant and audit contracts remain owned by Core/shared fabric. Cross-system synchronization belongs to TaskBridge where synchronization is required.

## Migration policy
No existing Core module is removed, renamed, or migrated by this bootstrap. Migration requires source inventory, schema/API parity, test evidence, data migration and rollback plans, owner approval and an ADR.
