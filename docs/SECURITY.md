# Security Baseline

## Mandatory controls
- Integrate with Core IAM and tenant isolation through verified contracts; deny by default.
- Enforce row-, column-, dataset- and metric-level authorization where sensitivity requires it.
- Classify PII, PHI, financial, employment, confidential and public data at ingestion and catalog layers.
- Minimize sensitive-data replication; use tokenized or pseudonymized analytical views where possible.
- Store secrets only in an approved secrets manager or protected runtime configuration; metadata contains aliases, never secret values.
- Encrypt network traffic and sensitive persistent storage; define key rotation and access logging.
- Maintain immutable or tamper-evident audit evidence for privileged access, exports, model runs and governed actions.
- Apply retention, deletion, residency and legal-hold policies by data class and jurisdiction.
- Protect exports, scheduled reports, caches, embedded dashboards and API responses against data leakage.
- Separate development/test data from production; prohibit unapproved production data in test fixtures.

## AI/model controls
- Track model, dataset, prompt/configuration, feature and evaluation versions.
- Record provenance, uncertainty, drift and limitations.
- Test for leakage, bias, unsafe inference and tenant boundary violations.
- Gate recommendations and actions by policy and autonomy level; human approval is default for consequential actions.

## Security status
This is a baseline specification. No security certification, penetration test or production control implementation is claimed.
