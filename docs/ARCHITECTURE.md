# Architecture

## Architectural intent
A federated, contract-first BI platform that converts governed source data into trusted semantic models, metrics, analysis and decision support. It should support self-hosted deployments and modular adapters without forcing every workload into one technology.

## Logical planes
1. **Source and ingestion plane** — source registry, connector contracts, ingestion manifests, CDC/batch/stream adapters, schema evolution and quarantine.
2. **Data product plane** — curated datasets, ownership, quality, classification, retention and data-product publication.
3. **Storage and compute plane** — pluggable operational staging, analytical warehouse/lakehouse and query engines. Technology choices remain open pending ADR.
4. **Semantic plane** — dimensions, facts, entities, measures, metric definitions, business calendars, hierarchies, calculation semantics and certified datasets.
5. **Analytics plane** — descriptive/diagnostic analytics, forecasting, anomaly detection, optimization, scenario simulation and model evaluation.
6. **Experience plane** — dashboards, reports, exploration, alerts, embedded analytics and APIs.
7. **Decision plane** — recommendations, alternatives, approvals, decision records, controlled actions and outcome feedback.
8. **Governance/control plane** — identity, tenant isolation, policy, lineage, catalog, audit, quality, observability, cost and lifecycle.

## Shared enterprise fabric
Use Core IAM, tenant, audit, notification, integration/API gateway and other shared services through versioned contracts after compatibility is verified. EBMA is mandatory. UPM declares; UAPC compiles; Build Orchesty executes approved plans; n8n coordinates; TaskBridge synchronizes explicitly.

## Data flow
Source systems → connector/ingestion → validation/quarantine → governed data product → semantic model → metric/query → analysis/model/simulation → dashboard/report/recommendation → approved action → outcome/learning.

Every transformation should preserve source provenance, timestamps, schema/version identity, tenant scope, quality results and lineage.

## Design constraints
- Operational source systems remain authoritative for their records.
- Avoid uncontrolled copies of sensitive data.
- Metric definitions are versioned and governed.
- No raw credentials in metadata or logs.
- Model outputs are not facts until validated and labelled.
- High-impact actions require policy checks and human approval unless an explicitly approved autonomy profile permits otherwise.
- Support deployment portability; do not assume a single cloud provider.

## Implementation status
This document is target architecture, not evidence that any of these planes are implemented in this repository.
