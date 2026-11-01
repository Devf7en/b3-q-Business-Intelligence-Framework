# ADR-0001: Independent BI Product Boundary and Core Reconciliation

- **Status:** Accepted as initial documentation decision
- **Date:** 2026-11-01

## Context
b3Ɛq Core already documents BI module 104300 and ETL module 104450. The BI module includes source/dataset, mart/dimension/fact/metric, dashboard/widget, report/schedule, model/run/prediction, catalog, quality and alert metadata. Its README explicitly says it is a catalog/registry rather than a warehouse, rendering, training or email execution engine. The ETL module documents pipeline metadata, stages, versions, jobs/runs, transforms, profiling, lineage, dependencies and alerts; its README describes metadata/orchestration rather than an execution engine.

## Decision
Create an independent BI Framework repository to own product architecture, semantic/metric contracts, capability roadmap and lifecycle. Preserve Core as current runtime host and owner of existing BI/ETL capabilities until an evidence-based migration decision is approved. Avoid duplicating registries or asserting that a separate runtime already exists.

## Consequences
- Source inventory and runtime verification are P0.
- Existing Core schemas, rights, APIs, tests and data must be mapped before extraction.
- Product contracts may be designed here but must be versioned and reviewed with Core/shared-fabric owners.
- Migration requires explicit approval, compatibility tests, data migration, rollback and documentation.
- This ADR does not authorize code movement or removal of Core modules.
