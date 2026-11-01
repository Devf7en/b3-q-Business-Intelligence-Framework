# Roadmap

## P0 — Evidence and boundary reconciliation
- Inventory Core BI 104300 and ETL 104450 source files, schemas, rights, APIs, tests and runtime behavior.
- Reconcile module registry versions against descriptors and source.
- Decide retain/adapt/extract/replace per capability; Core remains authoritative until approved.
- Recover all prior BI-specific requirements and assets.
- Correct repository visibility to Private.

## P1 — Canonical contracts
- Define data-product, dataset, metric, semantic-model, lineage, quality and ingestion contracts.
- Establish identity, tenant, audit and classification integration.
- Define schema/version compatibility and contract tests.

## P2 — Reference architecture and vertical slice
- Select storage/query/semantic/visualization components through ADRs.
- Implement one source-to-certified-metric-to-dashboard vertical slice.
- Demonstrate tenant isolation, row/column policy, lineage and reproducible refresh.
- Establish automated tests and CI.

## P3 — Analytics and decision intelligence
- Add forecasting, anomaly detection, scenario simulation and evaluation.
- Add governed recommendations, approvals, action dispatch and outcome learning.
- Integrate with approved AI/model services.

## P4 — Enterprise rollout
- Add portfolio-wide data products, connectors, deployment profiles and operational SLOs.
- Complete threat modelling, security testing, backup/restore and DR exercises.
- Assess EBMA conformance with evidence before claiming conformance.

Roadmap gates are evidence-driven; dates and completion claims require actual delivery records.
