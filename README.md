# Kaggle / field notes

A public research portfolio for competitive machine learning. It records the method behind the work: the baseline, the validation checks, the experiments that failed, and the results once they can be pointed at.

<p align="center">
  <img src="assets/research-atlas.svg" alt="Diagram of the method: evidence, experiment, systems, and public proof, with boundary and retrospective alongside" width="100%" />
</p>

<p align="center"><sub>Diagram of the method. Drawn for this repository, not a screenshot of a run.</sub></p>

Profile: [kaggle.com/pascalledesma](https://www.kaggle.com/pascalledesma)

## Where to read

| File | What it holds |
| :-- | :-- |
| [docs/EVIDENCE_LEDGER.md](docs/EVIDENCE_LEDGER.md) | Each claim, its source, the date it was read |
| [docs/JOURNEY.md](docs/JOURNEY.md) | How the practice moved from disconnected runs to a repeatable routine |
| [docs/EXPERIMENT_LEARNING_MAP.md](docs/EXPERIMENT_LEARNING_MAP.md) | How a hypothesis gains or loses confidence |
| [docs/COMPETITION_INDEX.md](docs/COMPETITION_INDEX.md) | The format for a competition record, published after review |
| [data/public-profile-snapshot.csv](data/public-profile-snapshot.csv) | A sparse, dated data layer |

## What is verified

The public account at [kaggle.com/pascalledesma](https://www.kaggle.com/pascalledesma) exists and is mine. The engineering practice is documented: disposable compute, credential isolation, readiness checks, a baseline before any model tuning, and a validation routine that tries to break the split before trusting it.

Current rank, medals, points, placements, scores, competition dates and notebook counts are not stated here. Each of those moves from blank to visible through a dated source in the [evidence ledger](docs/EVIDENCE_LEDGER.md), and not before.

## The loop

```mermaid
flowchart LR
    classDef proof fill:#0F172A,color:#FFFFFF,stroke:#38BDF8,stroke-width:2px
    classDef work fill:#172554,color:#DBEAFE,stroke:#60A5FA,stroke-width:2px
    classDef check fill:#3F1D5B,color:#F3E8FF,stroke:#C084FC,stroke-width:2px
    classDef boundary fill:#1F2937,color:#F9FAFB,stroke:#94A3B8,stroke-dasharray: 5 5

    R[Read the rules<br/>and metric]:::proof --> B[Build an end-to-end<br/>baseline]:::work
    B --> V[Mirror the metric in<br/>local validation]:::check
    V --> H[Write one falsifiable<br/>hypothesis]:::work
    H --> X[Run it and record<br/>the result]:::work
    X --> D{Does the signal<br/>hold up?}:::check
    D -->|yes| I[Refine the idea]:::proof
    D -->|no or unclear| A[Audit split, leakage,<br/>drift, variance]:::check
    A --> V
    I --> P[Publish what the<br/>rules allow]:::boundary
```

A higher number is not the only output. The other one is a chain of reasoning that survives someone trying to break it.

## What is public right now

| Signal | State | What it means | Gate |
| :-- | :--: | :-- | :-- |
| Profile identity | Verified | The Kaggle account is linked above. | Public profile |
| Competition stats | Awaiting capture | No rank, medals, points or counts are claimed. | Dated profile export |
| Competition records | Awaiting inventory | No names or placements are inferred from memory. | Public result page |
| Notebooks and datasets | Awaiting inventory | No artifact catalogue is implied. | Public artifact links |
| Experiment method | Documented | The baseline, validation and review loops are written down. | Public-safe engineering notes |

```mermaid
xychart-beta
    title "Evidence coverage, first public edition"
    x-axis ["Identity", "Method", "Profile stats", "Competition records", "Artifact inventory"]
    y-axis "Publication readiness" 0 --> 1
    bar [1, 1, 0, 0, 0]
```

This chart measures coverage, not performance. A zero means not yet evidenced.

## The four stations

```mermaid
mindmap
  root((Kaggle field notes))
    Evidence
      Dated sources
      Public links
      Claim ledger
    Experimentation
      Baselines
      Falsifiable hypotheses
      Validation incidents
    Systems
      Disposable compute
      Readiness checks
      Credential isolation
    Retrospectives
      Reusable lessons
      Rule-safe summaries
      Public proof
```

| Station | The question it asks | Read |
| :-- | :-- | :-- |
| Evidence | Can a reader verify this? | [Evidence ledger](docs/EVIDENCE_LEDGER.md) |
| Experimentation | What did the test actually teach? | [Experiment learning map](docs/EXPERIMENT_LEARNING_MAP.md) |
| Systems | Could the loop be repeated safely? | [Research journey](docs/JOURNEY.md) |
| Retrospectives | What is safe and useful to share? | [Competition index](docs/COMPETITION_INDEX.md) |

## The publishing rule

A page, number, chart or link goes public only after the [evidence ledger](docs/EVIDENCE_LEDGER.md) and the [public boundary](PUBLIC_BOUNDARIES.md) are both satisfied: source, date, permission, competition sensitivity. That keeps the private operating manual private, and keeps this repository readable by someone with no context.

<p align="center"><sub><a href="docs/EVIDENCE_LEDGER.md">Evidence ledger</a> · <a href="docs/JOURNEY.md">Journey</a> · <a href="docs/EXPERIMENT_LEARNING_MAP.md">Experiment map</a> · <a href="docs/COMPETITION_INDEX.md">Competition index</a> · <a href="PUBLIC_BOUNDARIES.md">Public boundaries</a></sub></p>
