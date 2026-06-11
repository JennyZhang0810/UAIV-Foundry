# UAIV-Foundry

**UAIV-Foundry** is a data production operating system for low-altitude multimodal datasets.

It is designed to support the full lifecycle of UAIV-style dataset construction:

```text
resource curation -> data planning -> annotation -> QA -> release -> benchmark -> iteration
```

This repository currently hosts the public project page for UAIV-Foundry. The full engineering codebase and dataset release materials are being organized and will be released progressively after annotation, review, and final quality checks are complete.

## What Is UAIV-Foundry?

UAIV-Foundry is not just an awesome list, and it is not another annotation platform.

It is the infrastructure layer around low-altitude data production:

- **Knowledge Layer**: structured resources for annotation platforms, UAV/remote-sensing datasets, data quality tools, synthetic-data workflows, and remote-sensing VLMs.
- **Data Factory Layer**: manifest generation, Golden Dataset calibration, worker assignment, Labeler import records, export intake, QA gates, rework plans, and dashboards.
- **Release & Benchmark Layer**: dataset cards, release readiness checks, public-package planning, benchmark request protocols, metric specs, and failure-to-data feedback.

## UAIV Ecosystem

UAIV-Foundry works together with two other UAIV components:

| Component | Role |
| --- | --- |
| **UAIV-Real** | The low-altitude multimodal dataset/product. |
| **UAIV-Labeler** | The human annotation workbench for scene labels, object boxes, OCR, event QA, environment state, and review. |
| **UAIV-Foundry** | The data production OS that organizes, audits, documents, releases, and benchmarks the dataset. |

## Current First-Public Batch

The current first-public candidate focuses on low-altitude city-governance imagery.

| Item | Current Status |
| --- | --- |
| Cleaned images | 4,796 |
| Total files in first-public scope | 5,019 |
| Golden Dataset | 96 images prepared |
| Worker groups | 12 groups planned |
| Annotation | pending |
| Final QA | pending |
| Public release | pending |
| Real benchmark | pending |

Current status:

```text
pre-release engineering status
```

This page does **not** claim that UAIV-Real has been publicly released. Reviewed annotations, final QA, license decisions, public download links, and real benchmark results are still pending.

## Why It Matters

Low-altitude dataset construction is not only image collection. A reliable dataset also needs:

- reproducible data scope and manifest records;
- annotation guidelines and Golden Dataset calibration;
- export intake and structural validation;
- task-specific QA gates;
- rework closure records;
- dataset cards and release checks;
- benchmark protocols aligned with released data;
- failure analysis that feeds back into the next data iteration.

UAIV-Foundry makes these steps explicit, auditable, and reusable.

## Project Page

The current project page is:

```text
index.html
```

It introduces:

- what UAIV-Foundry is;
- how it relates to UAIV-Real and UAIV-Labeler;
- the current first-public city-governance batch;
- the closed-loop data production process;
- release gates and pending blockers;
- the long-term value of Foundry as data infrastructure.

## Roadmap

- [x] Build initial project page.
- [x] Define Foundry, UAIV-Real, and UAIV-Labeler roles.
- [x] Prepare first-public manifest, Golden subset, and worker-group plan.
- [x] Prepare QA, release, dashboard, and benchmark dry-run protocols.
- [ ] Finish Golden Dataset annotation and QA.
- [ ] Finish full annotation, review, and rework closure.
- [ ] Publish final dataset card, release package, and public links.
- [ ] Run real benchmark with reviewed annotations.
- [ ] Release the full Foundry engineering repository.

## Citation and Release Status

This page is the initial public-facing project page for UAIV-Foundry. Please do not treat it as a final dataset release or benchmark leaderboard.

Formal citation, dataset license, and download links will be added after the first public data release is complete.
