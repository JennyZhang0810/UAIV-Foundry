# UAIV-Foundry

**UAIV-Foundry** is the public project-page package for the UAIV data production operating system.

It explains how low-altitude datasets are not only collected and annotated, but also organized for QA, release readiness, dataset cards, benchmark protocols, and later iteration.

It is designed to support the full lifecycle of UAIV-style dataset construction:

```text
resource curation -> data planning -> annotation -> QA -> release -> benchmark -> iteration
```

This directory is the **public release package** for the Foundry project page.

Use it when you want the final public-facing GitHub Pages version.

Do not confuse it with:

- `docs/site/`: local working source for iteration and internal review
- repository root `README.md`: engineering repository homepage for the full Foundry workspace

## What Is UAIV-Foundry?

UAIV-Foundry is not just an awesome list, and it is not another annotation platform.

It is the infrastructure layer around low-altitude data production:

- **Knowledge Layer**: structured resources for annotation platforms, UAV/remote-sensing datasets, data quality tools, synthetic-data workflows, and remote-sensing VLMs.
- **Data Factory Layer**: manifest generation, Golden Dataset calibration, worker assignment, Labeler import records, export intake, QA gates, rework plans, and dashboards.
- **Release & Benchmark Layer**: dataset cards, release readiness checks, public-package planning, benchmark request protocols, metric specs, and failure-to-data feedback.

## UAIV Ecosystem

UAIV-Foundry works together with two other UAIV components:

| Component | Role | Public Entry Points |
| --- | --- | --- |
| **UAIV-Real / UAIV Dataset** | The low-altitude multimodal dataset/product. | [Project Page](https://jennyzhang0810.github.io/LowAltitude-Multimodal-Dataset/) · [GitHub](https://github.com/JennyZhang0810/LowAltitude-Multimodal-Dataset) · [ScienceDB](https://www.scidb.cn/detail?dataSetId=203705443be44f7882bb9ddfd7d401da) |
| **UAIV-Labeler** | The human annotation workbench for scene labels, object boxes, OCR, event QA, environment state, and review. | [Project Page](https://jennyzhang0810.github.io/UAIV-Labeler/) · [GitHub](https://github.com/JennyZhang0810/UAIV-Labeler) · [Live Demo](http://8.137.184.86/) |
| **UAIV-Foundry** | The data production OS that organizes, audits, documents, releases, and benchmarks the dataset. | [Project Page](https://jennyzhang0810.github.io/UAIV-Foundry/) · [GitHub](https://github.com/JennyZhang0810/UAIV-Foundry) |

In short:

```text
UAIV-Real is what we release.
UAIV-Labeler is where humans annotate.
UAIV-Foundry is how we make the production process auditable, measurable, and reusable.
```

## Current First-Public Batch

The current first-public candidate focuses on low-altitude city-governance imagery.

| Item | Current Status |
| --- | --- |
| Source-image pool | 4,796 |
| Standardized task records | 5,088 |
| Split families | development + grouped benchmark |
| Audit package | duplicate / near-duplicate / bbox / label cleanup ready |
| Public deposition | pending |
| Final privacy counts | pending |
| Real benchmark | pending reviewed public release |

Current status:

```text
pre-release engineering status
```

This page does **not** claim that UAIV-Real CityGov has completed public deposition. DOI/accession, final public links, and final privacy-release counts are still pending.

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

Formal citation, public deposition information, and final release links will be added after the public data release is completed.
