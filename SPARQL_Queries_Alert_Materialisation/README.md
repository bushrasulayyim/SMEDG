# SPARQL Alert Materialisation

This folder contains SPARQL queries used to materialise governance alerts as persistent ontology instances within the SMEDG framework.

## Purpose

These queries are responsible for transforming detected policy violations into machine-readable `Alert` entities stored in the knowledge graph. Unlike SHACL validation results, which are transient, these SPARQL updates persist violations in a dedicated alerts graph, enabling monitoring, dashboards, and audit trails.

## What this folder contains

### `SPARQL_Alert_Materialisation.ttl`

This file contains SPARQL UPDATE statements that:

- Detect policy violations for Competency Questions (CQ1–CQ24),
- Create instances of `smedg:Alert`,
- Store alerts in the `<urn:smedg:alerts>` named graph,
- Record:
  - Violated policy clause (e.g., P1),
  - Triggering CQ and SHACL shape,
  - Offending asset or event,
  - Severity level,
  - Explanation of the violation,
  - Recommended corrective action,
  - Detection timestamp.

## How it relates to SHACL

- **SHACL** defines the formal policy constraints and performs validation.
- **SPARQL** implements alert materialisation by persisting violations detected conceptually by those constraints.
- Alerts reference the originating SHACL shapes using shared identifiers (e.g., `smedg:CQ01_ConfidentialAsset_StorageShape`), ensuring traceability from policy → CQ → shape → alert.

## Usage

These SPARQL queries are executed after validation to:

- Populate the alert graph,
- Support reporting and dashboards,
- Enable auditability and governance workflows.

The alerts generated here are later retrieved by the user interface through reporting queries in the View layer.

## Traceability

Each alert instance is traceable through: Policy Clause → Competency Question → SHACL Shape → SPARQL Alert → Dashboard. This supports explainable and operational governance suitable for SME environments.


