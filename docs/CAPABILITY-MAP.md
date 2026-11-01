# Capability Map

| Capability | Target responsibility | Initial state |
|---|---|---|
| Data source registry | Systems, owners, connection aliases, scopes | Existing Core BI metadata; reconcile |
| Dataset/data-product catalog | Dataset contracts, owner, classification, quality | Existing Core catalog baseline; expand |
| Ingestion/connectors | Batch, CDC, streaming, API and file ingestion | Planned; Core API Gateway/ETL are adjacent |
| Warehouse/lakehouse | Persist analytical data and snapshots | Not verified in Core BI |
| Semantic modeling | Facts, dimensions, grain, relationships, measures | Core metadata baseline |
| Metrics/KPI governance | Formula, owner, target, thresholds, versions | Core BI metric metadata |
| Dashboards/widgets | Visualization definitions and delivery | Core catalog exists; renderer not established by BI README |
| Reporting/distribution | Reports, schedules, subscriptions | Core metadata exists; delivery engine not established |
| Forecasting/ML | Model registry, training/scoring, evaluation, predictions | Core metadata registries exist; execution not established |
| Quality/profiling | Rules, profiling, assertions, incidents | Core BI/ETL metadata baseline |
| Lineage | Source-to-consumption graph and impact analysis | ETL lineage metadata baseline |
| Alerts | Thresholds, anomalies, routed notifications | Core alert metadata baseline |
| Simulation | Scenarios, assumptions, uncertainty, sensitivity | Planned |
| Decision intelligence | Alternatives, evidence, approvals, outcomes | Planned |
| Governance | IAM, tenant, audit, privacy, retention | Shared Core services; integration verification required |
| AI-native cycle | Observe, Understand, Predict, Recommend, Simulate, Act, Learn | Required design principle; implementation pending |
| Observability | Freshness, latency, quality, cost, service health | Planned |
| Embedded BI/API | Governed query and presentation interfaces | Planned |

Capability status is a discovery baseline. Do not infer runtime completeness from registry rows or module status labels.
