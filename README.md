# b3Ɛq Business Intelligence Framework™
**Repository:** `Devf7en/b3-q-Business-Intelligence-Framework`  
**Version:** 0.1.0  
**Portfolio ID:** B3EQ-PORT-0024  
**Lifecycle:** discovery / architecture bootstrap  
**EBMA conformance:** not_assessed  
**Repository visibility:** GitHub currently reports Public; portfolio policy requires Private. Owner action required.

## Purpose
An enterprise-grade, AI-native Business Intelligence Framework for transforming distributed enterprise data into trusted information, analytics, intelligence and governed decisions. It defines reusable contracts and architecture for data integration, semantic modeling, metrics, reporting, dashboards, advanced analytics, forecasting, simulation, decision intelligence, data governance and enterprise-wide performance management.

## Existing Core capability — preserve and reconcile
Core already records BI module 104300 v1.1.1 and ETL module 104450 v1.1.0. The BI module documents data-source and dataset registries; warehouse/semantic metadata (marts, dimensions, fact-table catalog, metrics); dashboard/widget catalogs; report/schedule catalogs; ML model/run/prediction registries; data catalog, quality checks and KPI alerting. The Core BI README explicitly describes a metadata/catalogue layer, not a physical warehouse, visualization engine, model-training engine or report-delivery engine. ETL records pipeline metadata, versions, stages, jobs/runs, transform/mapping rules, quality/profiling, lineage, dependencies and alerts; its README likewise describes metadata/orchestration rather than an execution engine.
These are source-repository findings, not a fresh runtime audit. Preserve Core as current owner until an approved extraction, adapter or migration decision is made.

## Authority and boundaries
- EBMA™ is the normative architecture authority.
- This repository owns the independent BI product architecture, semantic/metric contracts, BI capability roadmap and product lifecycle.
- b3Ɛq Core remains the shared runtime and current host of BI/ETL module capabilities pending migration approval.
- Core BI/ETL metadata must not be duplicated as competing sources of truth.
- DataOS projects own jurisdictional/data-domain stewardship; BI consumes governed data products and does not usurp their authority.
- KMS owns governed knowledge; BI owns analytical semantics and measured performance; Ethos Intelligence owns enterprise ethos/intent interpretation where approved.
- UPM declares platform composition; UAPC compiles validated intent; Build Orchesty executes approved plans; n8n coordinates workflows; TaskBridge performs explicit cross-system synchronization.
- Finance, SCM, TMS, HR, CRM and other vertical systems remain authoritative for their operational records.

## AI-first cycle
Observe → Understand → Predict → Recommend → Simulate → Act → Learn. Recommendations and actions require policy, provenance, authorization, approval and audit. No autonomous high-impact action is implied.

## Current truth
This repository begins with documentation and architecture contracts. No independent BI runtime, warehouse engine, connector, dashboard renderer, semantic query engine, model-training service, API, CI workflow, automated tests or production deployment is claimed.

## Documents
- [Architecture](docs/ARCHITECTURE.md)
- [Capability map](docs/CAPABILITY-MAP.md)
- [Boundaries and integrations](docs/BOUNDARIES-AND-INTEGRATIONS.md)
- [Security baseline](docs/SECURITY.md)
- [Operations baseline](docs/OPERATIONS.md)
- [Roadmap](docs/ROADMAP.md)
- [ADR-0001](docs/adr/ADR-0001-product-boundary-and-core-reconciliation.md)
- [Illustrative metric contract](contracts/metric-definition.example.yaml)
- [Ideation](ideation.mdc)
- [Conversation history](conversation.mdc)


## EBMA architecture and conformance

This project is governed by the b3Ɛq-wide EBMA adoption mandate. See [EBMA Adoption Notice](docs/EBMA-ADOPTION.md) and the [shared profile registry](https://github.com/Devf7en/b3-q_EBMA/blob/main/profiles/portfolio-profiles.json). This project is not currently declared EBMA-conformant.
