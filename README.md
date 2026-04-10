# Second Amendment Dependencies

An empirical investigation of how contemporary readers interpret sentences with syntactic structures analogous to the Second Amendment of the United States Constitution.

> *"A well regulated Militia, being necessary to the security of a free State, the right of the people to keep and bear Arms, shall not be infringed."*

## Overview

The Second Amendment contains a syntactic structure that has been debated for more than two centuries. A prefatory clause ("A well regulated Militia, being necessary to the security of a free State") is connected to an operative clause ("the right of the people to keep and bear Arms, shall not be infringed") by a participial phrase. Courts and scholars disagree about whether the prefatory clause *limits* the operative clause (a **conditional** reading) or merely *contextualizes* it (a **categorical** reading). This disagreement has driven landmark decisions from *Heller* (2008) through *Bruen* (2022) to *Rahimi* (2024).

This project isolates the syntactic question from the political one. We constructed sentences that mirror the Second Amendment's grammatical structure but address politically neutral topics (archives, weather stations, kitchens, harbors) and asked participants to interpret them.

## Research Questions

1. **Interpretation**: Do readers understand the "being necessary" construction as conditional (*only when* X is necessary) or categorical (*X is always necessary, therefore...*)?
2. **Rewrites**: When readers paraphrase the sentence in their own words, does conditional or categorical framing emerge?
3. **Confidence**: How confident are readers in their interpretation?
4. **Clause removal**: How does removing the prefatory clause change readers' understanding?
5. **Comma sensitivity**: Does comma placement affect perceived meaning?
6. **Causal vs. purposive**: Do readers interpret "being necessary" as expressing purpose ("for the purpose of") or factual causation ("because")?
7. **Individual differences**: Do gun control attitudes, age, or gender predict interpretation?

## Studies

### Pilot Study (Completed)

- **N** = 121 (after exclusions from 124 recruited)
- **Design**: Between-subjects; each participant read 1 of 20 sentences
- **Platform**: Qualtrics, recruited via Prolific
- **Key finding**: 84.3% of participants chose the categorical interpretation. Mean confidence was 5.20/7. Mixed-effects logistic regression confirmed this deviates from chance (*p* < .001).
- **Data and analysis**: Available in `Data/Pilot/` and `Code/R/Pilot/`

### Study 1A (In Progress)

- **Current N** = 100 analytic participants (104 collected, 4 excluded); target N = 300
- **Design**: Between-subjects; each participant reads 1 of 20 sentences
- **Platform**: Custom JavaScript experiment on Pavlovia, recruited via Prolific
- **Preregistered**: [AsPredicted](https://aspredicted.org/)

#### Key Results (Batch 1, N = 100)

| Finding | Result |
|---------|--------|
| Categorical interpretation rate | 90.5% (86/95 binary responders) |
| GLMM intercept | 2.44 log-odds, *p* < .0001 |
| Conditional rewrites produced | 0 out of 100 participants |
| Concordance (categorical FC) | 94.2% (81/86) |
| Concordance (conditional FC) | 0% (0/9) |
| Removal impact, categorical group | *M* = 3.22 (below midpoint, *p* < .0001) |
| Removal impact, conditional group | *M* = 4.33 (not different from midpoint, *p* = .70) |
| Distinguish: "because" | 61% chose "because" over "for the purpose of" |
| Comma Position 2 placement | 89% (before "the right of") |
| Comma Position 3 placement | 50% (before "must not be") |
| Gun control predicts interpretation | No (*p* = .25) |

#### Changes from Pilot

- Revised sentence stimuli (replaced 8 ceiling-effect items)
- Added AI detection (image-based CAPTCHA, self-paced reading)
- Added comma insertion task and comma variant comparisons
- Added "and" insertion impact question
- Added gun control attitudes measure
- Capitalized key phrases in interpretation options
- Counterbalanced Rewrite/AddCommas order
- Computational rewrite classification (Claude Sonnet 4, Anthropic API)

### Study 1B (Planned)

- Same design as 1A but with domain-specific technical vocabulary
- Tests whether interpretation patterns hold when readers cannot rely on real-world knowledge to resolve the sentence

## Stimuli

All 20 sentences in Study 1A follow the Second Amendment's structure: a prefatory clause with a "being necessary" construction, followed by an operative clause asserting a right.

| # | Sentence |
|---|----------|
| 1 | A well kept archive, being necessary for historical preservation, the right of people to access and manage records, must not be infringed. |
| 2 | A respected cultural tradition, being necessary for fostering unity within a community, the right of people to pass down and share knowledge, must not be infringed. |
| 3 | A properly organized marketplace, being necessary for economic exchange, the right of people to sell and trade goods, must not be revoked. |
| 4 | A well-supplied food reserve, being necessary for food security, the right of people to store and preserve essential provisions, must not be denied. |
| 5 | A consistently monitored weather station, being necessary for the prediction of dangerous storms, the right of people to prepare for and respond to natural threats, must not be violated. |
| 6 | A structurally sound dam, being necessary for protection from rising waters, the right of people to defend their land from flood, must not be revoked. |
| 7 | A tended field, being necessary for seasonal harvest, the right of people to cultivate and work the land, must not be infringed. |
| 8 | A replenished pharmacy, being necessary for the treatment of illness, the right of people to prepare and dispense medicine, must not be violated. |
| 9 | A functional kitchen, being necessary for meal preparation, the right of people to assemble and equip personal spaces for cooking, must not be infringed. |
| 10 | A community garden plot, being necessary for growing vegetables, the right of people to plant and cultivate their own produce, must not be infringed. |
| 11 | A dry basement, being necessary for storing household goods, the right of people to dig and waterproof spaces below the ground, must not be revoked. |
| 12 | A marked parking area, being necessary for the storage of vehicles, the right of people to park near their homes, must not be infringed. |
| 13 | A serviceable harbor, being necessary for access to water, the right of people to set anchors along the shore, must not be revoked. |
| 14 | A functioning legal system, being necessary for the administration of justice, the right of people to assemble and deliberate as jurors, must not be hindered. |
| 15 | A free press institution, being necessary for an informed public, the right of people to publish and distribute information, must not be impeded. |
| 16 | A representative town council, being necessary for local governance, the right of people to assemble and deliberate on civic matters, must not be violated. |
| 17 | A reliable postal network, being necessary for civic communication, the right of people to send and receive correspondence, must not be disrupted. |
| 18 | A working public bus system, being necessary for urban mobility, the right of people to plan and operate shared transportation, must not be revoked. |
| 19 | A consumer co-op, being necessary for fair access to goods, the right of people to pool purchasing power and govern enterprises jointly, must not be violated. |
| 20 | A trained group of medical responders, being necessary for public health emergencies, the right of people to study and practice emergency care, shall not be infringed. |

Sentence 20 uses "shall not" rather than "must not," mirroring the actual Second Amendment.

## Measures

Each participant sees one sentence and responds to the following. The Rewrite and AddCommas tasks are presented in randomized order.

**Rewrite** (open-ended): "Please rewrite this sentence in your own words, making it as simple as possible for others to understand."

**AddCommas** (open-ended): Sentence shown with commas stripped. Participants add commas where they think they belong.

**Interpretation** (forced choice): Categorical ("always necessary, therefore the right must never be restricted"), conditional ("only in those specific cases when the subject is necessary"), or "neither."

**Confidence** (1-7): "How confident are you in your choice above?"

**IsTrue** (conditional on interpretation = 1 or 3): "Assuming the sentence is correct, which of the following is true?" Three options ranging from "even if not crucial" to "only when absolutely essential." Skipped for categorical interpreters.

**Remove** (1-7): Impact of removing the prefatory clause (1 = same implications, 7 = completely different).

**And** (1-7): Impact of inserting "and" before the operative clause. Same scale.

**Comma comparisons** (4-point scale, three pairwise): 3-comma vs. 2-comma, 3-comma vs. 1-comma, 2-comma vs. 1-comma. Commas displayed as pipe symbols.

**Distinguish** (forced choice): "For the purpose of" vs. "Because" vs. "Neither."

**Demographics**: Gender, age, race, native language, English exposure, gun control attitudes, AI use, seriousness.

## Analysis Pipeline (Study 1A)

The analysis is structured as a four-stage pipeline with clean separation between data assembly, exclusions, classification, and hypothesis testing.

| Stage | File | Description |
|-------|------|-------------|
| 0 | `SA_E1A_Power_Analysis_v2.Rmd` | Power analysis for target N |
| 1 | `SA_E1A_Stage1_DataAssembly.Rmd` | Merge individual Pavlovia CSVs, join sentence metadata |
| 2 | `SA_E1A_Stage2_Exclusions.Rmd` | Sequential exclusion criteria per preregistration |
| 3 | `SA_E1A_Stage3_RewriteClassification.ipynb` | Blind LLM classification of rewrites (Python, Anthropic API) |
| 4 | `SA_E1A_Stage4_HypothesisTesting.Rmd` | All 7 preregistered hypotheses + exploratory analyses |
| Figs | `SA_E1A_PNAS_Figures.Rmd` | Publication-ready figures |

## Repository Structure

```
├── Code/
│   ├── R/
│   │   ├── Pilot/
│   │   │   ├── PilotAnalysis_Final.Rmd
│   │   │   └── PilotAnalysis_Final.html
│   │   └── Study1A/
│   │       ├── SA_E1A_Power_Analysis_v2.Rmd
│   │       ├── SA_E1A_Stage1_DataAssembly.Rmd
│   │       ├── SA_E1A_Stage2_Exclusions.Rmd
│   │       ├── SA_E1A_Stage4_HypothesisTesting.Rmd
│   │       └── SA_E1A_PNAS_Figures.Rmd
│   └── Python/
│       └── Study1A/
│           └── SA_E1A_Stage3_RewriteClassification.ipynb
├── Data/
│   ├── Pilot/
│   │   ├── Cleaned_Numeric_Second_Amendment_Dependencies_Pilot.csv
│   │   ├── Cleaned_Response_Second_Amendment_Dependencies_Pilot.csv
│   │   └── q1_rewrite_responses_for_coding.csv
│   └── Study1A/
│       ├── SA_E1A_analytic.csv
│       ├── SA_E1A_merged.csv
│       ├── SA_E1A_merged_with_exclusions.csv
│       └── SA_E1A_rewrite_classifications.csv
├── Docs/
│   ├── Memos/
│   └── Experiment/
├── Figures/
│   ├── Pilot/
│   └── Study1A/
│       ├── Fig1.pdf    (Interpretation distribution)
│       ├── Fig2.pdf    (Comma sensitivity)
│       ├── Fig3.pdf    (Confidence by group)
│       ├── Fig4.pdf    (Concordance heatmap)
│       ├── Fig5.pdf    (Removal impact by group)
│       ├── Fig6.pdf    (Removal impact overall)
│       └── Fig7.pdf    (Comma placement positions)
├── .gitignore
├── _config.yml
├── index.md
└── README.md
```

## Exclusion Criteria (Study 1A)

Applied sequentially before any hypothesis testing:

1. Test or incomplete runs
2. Failed CAPTCHA
3. Implausible self-paced reading times (< 100 ms minimum word-level RT)
4. Near-verbatim rewrite (Levenshtein edit distance < 5)
5. Self-reported non-seriousness
6. Self-reported AI use
7. Non-consent or mobile device
8. Total completion time under 3 minutes

## Recruitment

Participants are recruited through [Prolific](https://www.prolific.co/) with the following criteria:

- United States only
- Native English speaker or learned English before age 7
- Representative sample on political affiliation and ethnicity
- Desktop computer required

## Ethics

This research was approved by the UCLA Institutional Review Board. All participants provide informed consent and are debriefed at the conclusion of the study.

## Authors

**David G. Kamper** -- University of California, Los Angeles; University of Chicago Law School
Corresponding author: [davidgkamper@ucla.edu](mailto:davidgkamper@ucla.edu)

**Anna Walburger** -- University of California, Los Angeles

**Idan Blank** -- University of California, Los Angeles, Department of Psychology; Brain Research Institute

### CRediT Author Statement

| Role | Contributors |
|------|-------------|
| Conceptualization | David G. Kamper, Idan Blank |
| Methodology | David G. Kamper, Idan Blank |
| Software | David G. Kamper |
| Formal Analysis | David G. Kamper |
| Investigation | David G. Kamper, Anna Walburger |
| Data Curation | David G. Kamper, Anna Walburger |
| Writing | David G. Kamper |
| Review and Editing | Idan Blank |
| Visualization | David G. Kamper |
| Supervision | Idan Blank |
| Project Administration | David G. Kamper |

## License

This repository is intended for academic research purposes. Please contact the authors before reusing data or materials.

## Citation

> Kamper, D. G., Walburger, A., & Blank, I. (2025). Two centuries of debate over a sentence that readers find unambiguous. Manuscript in preparation, University of California, Los Angeles.
