# KAGGLE / FIELD NOTES

> **A public research portfolio for competitive machine learning.**
>
> Not a trophy cabinet. Not a notebook dump. A living record of how a serious practice is built: establish the baseline, challenge the validation, preserve the learning, then earn the right to make a claim.

<p align="center">
  <img src="assets/research-atlas.svg" alt="Kaggle Field Notes research atlas: evidence, experiments, systems, and public proof" width="100%" />
</p>

<p align="center">
  <a href="https://www.kaggle.com/pascalledesma"><img src="https://img.shields.io/badge/Kaggle-Pascal-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle profile" /></a>
  <a href="docs/EVIDENCE_LEDGER.md"><img src="https://img.shields.io/badge/claim--standard-source--backed-111827?style=for-the-badge" alt="Source backed claims" /></a>
  <a href="PUBLIC_BOUNDARIES.md"><img src="https://img.shields.io/badge/public--surface-intentionally%20redacted-7C3AED?style=for-the-badge" alt="Public safe by design" /></a>
</p>

---

## Enter the research room

| Read this | You will find | Why it exists |
| :-- | :-- | :-- |
| **[01 · Evidence ledger](docs/EVIDENCE_LEDGER.md)** | The difference between verified signal and future evidence. | Keeps the portfolio honest when the internet is vague. |
| **[02 · Research journey](docs/JOURNEY.md)** | The evolution from runs to a repeatable practice. | Gives the work a narrative without inventing a scoreboard. |
| **[03 · Experiment map](docs/EXPERIMENT_LEARNING_MAP.md)** | How a hypothesis earns, loses, or revises confidence. | Makes method visible. |
| **[04 · Competition atlas](docs/COMPETITION_INDEX.md)** | The structure for public, post-review competition records. | Makes future depth navigable. |
| **[05 · Source snapshot](data/public-profile-snapshot.csv)** | A deliberately sparse, dated data layer. | Makes omissions explicit rather than decorative. |

<details>
<summary><strong>What is verified right now?</strong></summary>

The public Kaggle account is identifiable as [Pascal](https://www.kaggle.com/pascalledesma). This first release also documents the engineering practice behind the work: disposable compute, credential isolation, readiness checks, baseline-first experiments, and validation discipline.

It does **not** claim current rank, medals, points, placements, scores, competition dates, or notebook inventory. Those move from blank to visible only through a dated source in the [evidence ledger](docs/EVIDENCE_LEDGER.md). Restraint: still a feature, even on GitHub.

</details>

---

## The machine behind the learning

```mermaid
flowchart LR
    classDef proof fill:#0F172A,color:#FFFFFF,stroke:#38BDF8,stroke-width:2px
    classDef work fill:#172554,color:#DBEAFE,stroke:#60A5FA,stroke-width:2px
    classDef check fill:#3F1D5B,color:#F3E8FF,stroke:#C084FC,stroke-width:2px
    classDef boundary fill:#1F2937,color:#F9FAFB,stroke:#94A3B8,stroke-dasharray: 5 5

    R[Read the rules<br/>and metric]:::proof --> B[Build an end-to-end<br/>baseline]:::work
    B --> V[Mirror the metric in<br/>local validation]:::check
    V --> H[Write one falsifiable<br/>hypothesis]:::work
    H --> X[Run + record<br/>the experiment]:::work
    X --> D{Does the signal<br/>hold up?}:::check
    D -->|yes| I[Refine the idea]:::proof
    D -->|no / unclear| A[Audit split, leakage,<br/>drift, and variance]:::check
    A --> V
    I --> P[Publish only the<br/>permitted learning]:::boundary
```

The artifact is not merely a higher number. It is a chain of reasoning that can survive someone trying to break it.

---

## Research surface · current edition

| Signal | Public state | What it means | Evidence gate |
| :-- | :--: | :-- | :-- |
| Profile identity | **Verified** | The public Kaggle identity is linked above. | Public profile |
| Competition stats | **Awaiting capture** | No ranks, medals, points, or counts are claimed. | Dated profile export |
| Competition records | **Awaiting inventory** | No names or placements are inferred from memory. | Public result or team page |
| Public notebooks / datasets | **Awaiting inventory** | No artifact catalogue is implied. | Public artifact links |
| Experiment doctrine | **Documented** | Baseline, validation, and learning loops are recorded. | Public-safe engineering evidence |

```mermaid
xychart-beta
    title "Evidence coverage — first public edition"
    x-axis ["Identity", "Method", "Profile stats", "Competition records", "Artifact inventory"]
    y-axis "Publication readiness" 0 --> 1
    bar [1, 1, 0, 0, 0]
```

This is a coverage chart, not a performance chart. A zero here means **not yet evidenced**, not “nothing happened.”

---

## Four stations, one discipline

```mermaid
mindmap
  root((Kaggle\nField Notes))
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

| Station | The question it asks | Explore |
| :-- | :-- | :-- |
| **Evidence** | “Can a reader verify this?” | [Evidence ledger](docs/EVIDENCE_LEDGER.md) |
| **Experimentation** | “What did the test actually teach?” | [Experiment learning map](docs/EXPERIMENT_LEARNING_MAP.md) |
| **Systems** | “Could the loop be repeated safely?” | [Research journey](docs/JOURNEY.md) |
| **Retrospectives** | “What is safe and useful to share?” | [Competition atlas](docs/COMPETITION_INDEX.md) |

---

## The public contract

The useful story is the **problem → decisive test → lesson → proof**. The private operating manual remains private.

Before a new page, number, chart, or link is published, it passes the [evidence ledger](docs/EVIDENCE_LEDGER.md) and the [public boundary](PUBLIC_BOUNDARIES.md): source, date, permission, and competition sensitivity. This keeps the portfolio legible to collaborators and useful to future me without leaking credentials, private data, unreleased models, or live competition strategy.

---

<p align="center">
  <strong>Begin with the evidence. Follow the learning. Add the results when they can be proved.</strong><br/>
  <sub>[Evidence ledger](docs/EVIDENCE_LEDGER.md) · [Journey](docs/JOURNEY.md) · [Experiment map](docs/EXPERIMENT_LEARNING_MAP.md) · [Competition atlas](docs/COMPETITION_INDEX.md) · [Public boundaries](PUBLIC_BOUNDARIES.md)</sub>
</p>
