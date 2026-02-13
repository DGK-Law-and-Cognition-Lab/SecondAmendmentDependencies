# Second Amendment Dependencies

An empirical investigation of how contemporary readers interpret sentences with syntactic structures analogous to the Second Amendment of the United States Constitution.

> *"A well regulated Militia, being necessary to the security of a free State, the right of the people to keep and bear Arms, shall not be infringed."*

## Overview

The Second Amendment's unusual syntactic structure—a prefatory clause connected to an operative clause by a "being necessary" construction—has been at the center of decades of legal debate. Courts, scholars, and advocates have disagreed about whether the prefatory clause *limits* the operative clause (a **conditional** reading) or merely *explains* it (a **categorical** reading). Yet no empirical study has asked: how do ordinary readers actually interpret this structure?

This project isolates the syntactic question from the political one. We created sentences that mirror the Second Amendment's grammatical structure but address politically neutral topics—archives, weather stations, kitchens, harbors—and asked participants to interpret them. The central question is whether readers treat the "being necessary" clause as establishing a condition under which the right applies, or as a categorical assertion that the subject is always necessary and the right therefore must never be infringed.

## Research Questions

1. **Rephrasing**: How do readers restate the sentence in their own words? Does the rewrite reveal a conditional or categorical understanding?
2. **Interpretation of "Being Necessary" Clauses**: Do readers understand the construction as conditional (*only when* X is necessary) or categorical (*X is always necessary, therefore…*)?
3. **Confidence**: How confident are readers in their interpretation?
4. **Perceived Dependency**: To what extent do readers see the operative clause as dependent on or limited by the prefatory clause?
5. **Impact of Clause Removal**: How does removing the prefatory clause change readers' understanding of the operative clause?
6. **Comma Sensitivity**: Does the placement of commas affect interpretation?
7. **Causal vs. Purposive Distinction**: Do readers interpret the prefatory clause as expressing purpose ("for the purpose of") or factual causation ("because it is known that")?

## Studies

### Pilot Study (Completed)

- **N** = 121 (after exclusions from 124 recruited)
- **Design**: Between-subjects; each participant saw 1 of 20 sentences
- **Platform**: Qualtrics, recruited via Prolific
- **Key Finding**: 84.3% of participants chose the categorical interpretation ("always necessary"). Mean confidence was 5.20/7. Mixed-effects logistic regression confirmed this significantly deviates from chance (*p* < .001).
- **Data**: Available in `Data/`

### Study 1A — Non-Technical Sentences (In Progress)

- **Design**: Between-subjects; each participant sees 1 of 20 sentences with comma manipulation as the primary experimental variable
- **Platform**: Custom HTML experiment deployed on Pavlovia, recruited via Prolific
- **Changes from Pilot**: Updated sentence stimuli, randomized Rewrite/AddCommas order, capitalized key phrases in interpretation options, pipe-symbol comma comparisons with explicit transformation descriptions, added AI detection measures, added gun control attitudes measure
- **Sentences**: See [Stimuli](#stimuli) below

### Study 1B — Technical Sentences (Planned)

- Same design as 1A but with domain-specific terminology that participants are unlikely to have prior knowledge about
- Intended to test whether interpretation patterns hold when readers cannot rely on real-world knowledge to resolve the sentence

## Stimuli

All 20 sentences in Study 1A follow the Second Amendment's structure: a prefatory clause with a "being necessary" construction, followed by an operative clause asserting a right that must not be violated.

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

Note: Sentence 20 uses "shall not" rather than "must not," mirroring the actual Second Amendment phrasing.

## Measures

Each participant sees one randomly assigned sentence and responds to the following questions in order. The first two tasks (Rewrite and AddCommas) are presented in randomized order across participants.

### Rewrite (Open-Ended)
> "Please rewrite this sentence in your own words, making it as simple as possible for others to understand."

### AddCommas (Open-Ended)
> "Here is the same sentence with all commas removed. Please copy the sentence below and add commas where you think they should go, without changing the meaning of the sentence. You may add zero or more commas."

Copy-paste is enabled for this question only. A 10-second minimum page timer is enforced.

### Interpretation (Forced Choice)
> "Regardless of your personal opinion or what is objectively true, what do you think the person who wrote the sentence meant?"

1. The right of [people] to [action] [must/shall] not be [verb] **ONLY IN THOSE SPECIFIC CASES** when [subject] is necessary for [purpose].
2. [Subject] are **ALWAYS** necessary for [purpose]. Therefore, the right of [people] to [action] must **NEVER** be [verb].
3. Neither of these interpretations.

### Confidence (7-Point Scale)
> "How confident are you in your choice above?"

Not at all confident (1) — Extremely confident (7)

### IsTrue (Conditional on Interpretation = 1 or 3)
> "Assuming the sentence is correct (regardless of your personal opinion), which of the following is true?"

1. The right must not be [verb] **EVEN IF** [subject] are **NOT CRUCIAL** for [purpose].
2. The right must not be [verb] **ONLY IN CASES** when [subject] are **AT LEAST SOMEWHAT IMPORTANT** for [purpose].
3. The right must not be [verb] **ONLY IN CASES** when [subject] are **ABSOLUTELY ESSENTIAL** for [purpose].

This question is skipped if the participant chose interpretation (2) ("always necessary"), since the answer would be logically entailed.

### Remove (7-Point Scale)
> "Imagine we removed the beginning of the sentence, and instead wrote: '[operative clause only].' How different would the implications of this sentence be compared to the original sentence?"

Same implications (1) — Completely different implications (7)

### And (7-Point Scale)
> "Suppose we rephrased the sentence by adding the word **and** before the last clause…"

The word "and" is displayed in red with underline. Response scale identical to Remove.

### Comma Comparisons (3 Questions)

Commas are replaced with the pipe symbol `|` for visibility. Each comparison explicitly describes which comma was removed. Presented in the order: 3-comma vs. 2-comma, 3-comma vs. 1-comma, 2-comma vs. 1-comma.

> "In the sentences below, we have replaced commas with the symbol **|** for easier visibility. Please treat each **|** as if it were a comma."

Response options:
1. They mean exactly the same thing
2. They mean mostly the same thing with slight differences
3. They have somewhat different meanings
4. They have very different meanings

### Distinguish (Forced Choice)
> "Some people distinguish between two types of interpretation. Which comes closest to your interpretation?"

1. The right must not be [verb] **FOR THE PURPOSE OF** having [subject] necessary for [purpose].
2. The right must not be [verb] **BECAUSE** it is known that [subject] is necessary for [purpose].
3. Neither of these interpretations.

## Attention and Quality Checks

- **Attention Check 1** (pre-experiment): "What is your task in this study?" with 5 options; incorrect answer triggers instruction re-read and retry
- **Police Sentence Check** (post-experiment): Comprehension questions about "The police were called by a novelist who wanted them to arrest the photographer" — tests basic reading comprehension with 3 factual questions
- **Atlas Browser Detection**: Automatic detection and exclusion of ChatGPT's built-in browser
- **Copy-Paste Prevention**: Disabled on all text entry fields except AddCommas
- **Page Timers**: 10-second minimum on all question pages
- **AI Self-Report**: "Did you use any AI tool (such as ChatGPT, Claude, or similar) to help answer any of the questions in this study? Your answer will NOT affect your payment in any way."
- **Seriousness Check**: "Did you complete this experiment seriously throughout (without responding randomly)?"
- **Environment Check**: Quiet environment and distraction self-reports

## Demographics

- Gender (Male / Female / Nonbinary / Other / Prefer not to say)
- Age (open-ended)
- Race/ethnicity (multi-select: White or Caucasian, Black or African American, American Indian/Native American or Alaska Native, Asian, Native Hawaiian or Other Pacific Islander, Other, Prefer not to say)
- Country of birth (USA, Canada, UK, Australia, New Zealand, India, Other)
- Native language (open-ended)
- Age of first English exposure (open-ended)
- Other languages spoken with ages and frequency (open-ended)
- English usage frequency as percentage (open-ended)
- Speech/language/vision/reading/hearing diagnoses (Yes with explanation / No)
- Gun control attitudes: "In general, do you think gun laws should be made more strict, less strict, or kept as they are now?" (Much more strict / Somewhat more strict / Kept as they are / Somewhat less strict / Much less strict)

## Repository Structure

```
├── Code/
│   └── R/
│       └── Pilot/
│           ├── PilotAnalysis_Final.Rmd    # Main pilot analysis (R Markdown)
│           ├── PilotAnalysis_Final.html   # Rendered pilot analysis
│           ├── PilotAnalysis_V3.Rmd       # Earlier analysis version
│           └── PilotAnalysis_V3.html      # Rendered earlier version
├── Data/
│   ├── Cleaned_Numeric_Second Amendment Dependencies_Pilot.csv
│   ├── Cleaned_Response_Second Amendment Dependencies_Pilot.csv
│   └── q1_rewrite_responses_for_coding_edited.csv
├── Docs/
│   ├── Memos/
│   │   ├── V1_DGK_Memorandum_DependenciesSecondAmendment.docx
│   │   └── Second Amendment Stimuli.docx
│   └── Experiment/
│       └── Qualtrics.pdf                  # Full Qualtrics survey export
├── Figures/
│   ├── second_amendment_dependency.svg
│   ├── second_amendment_dependency_1.svg
│   └── second_amendment_dependency_2.svg
├── .gitignore
├── _config.yml
├── index.md
└── README.md
```

## Data Dictionary

### Pilot Data — Numeric Responses (`Cleaned_Numeric_...csv`)

| Variable | Description | Values |
|----------|-------------|--------|
| `ResponseId` | Unique Qualtrics response identifier | String |
| `Prolific` / `PROLIFIC_PID` | Participant's Prolific ID | String |
| `Finished` | Whether participant completed survey | 1 = Yes |
| `Duration (in seconds)` | Total time in survey | Integer |
| `RewriteN` | Open-ended rewrite of sentence N | Free text |
| `InterpretationN` | Interpretation choice for sentence N | 1 = Conditional, 2 = Categorical, 3 = Neither |
| `ConfidenceN` | Confidence in interpretation | 1–7 (Not at all – Extremely confident) |
| `IsTrueN` | Perceived truth conditional | 1 = Even if not crucial, 2 = At least somewhat important, 3 = Absolutely essential |
| `RemoveN` | Impact of prefatory clause removal | 1–7 (Same – Completely different) |
| `AttentionCheck1` | Pre-experiment attention check | 3 = Correct |
| `Police1` | Who called the police? | 2 = Correct (Novelist) |
| `Police2` | What were police asked to do? | 2 = Correct (Take someone to station) |
| `Police3` | What caused this event? | 2 = Correct (Novelist used photographer's picture) |
| `Seriousness` | Self-reported seriousness | 4 = Yes |
| `Gender` | Gender identity | 1–5 |
| `Age` | Participant age | Integer |
| `Race` | Race/ethnicity | Multi-select |

### Pilot Data — Coded Rewrites (`q1_rewrite_responses_for_coding_edited.csv`)

| Variable | Description | Values |
|----------|-------------|--------|
| `Rewrite` | Participant's rewrite of the sentence | Free text |
| `Analysis` | Coded interpretation from rewrite | "Always", "Not Always", "Ambiguous" |
| `Q2_Interpretation_factor` | Participant's explicit interpretation choice | "Always necessary", "Only in cases when necessary" |

## Exclusion Criteria

Participants are excluded from analysis if any of the following apply:

1. **Failed attention check**: `AttentionCheck1 ≠ 3`
2. **Failed comprehension**: Incorrect on 2+ of 3 Police questions
3. **Non-serious**: `Seriousness ≠ 4`
4. **Incomplete**: `Finished ≠ 1`

## Key Pilot Results

- **84.3%** of participants chose the categorical interpretation ("always necessary")
- Mean confidence: **5.20 / 7** (SD = 1.42)
- Mixed-effects logistic regression intercept: **1.68 log-odds** (*p* < .001)
- Concordance between explicit choice and coded rewrite: **65.8%** agreement
- 8 sentences showed 100% categorical interpretation (ceiling effects), motivating stimulus revision for Study 1

## Recruitment

Participants are recruited through [Prolific](https://www.prolific.co/) with the following screening criteria:

- Location: United States only
- Language: Native English speaker or learned English before age 7
- Representative sample on political affiliation and ethnicity

## Ethics

This research was approved by the UCLA Institutional Review Board. All participants provide informed consent prior to participation and are debriefed at the conclusion of the study.

## Authors

**David G. Kamper** — University of California, Los Angeles  
Corresponding author · [davidgkamper@ucla.edu](mailto:davidgkamper@ucla.edu)

**Idan Blank** — University of California, Los Angeles, Department of Psychology  
[iblank@psych.ucla.edu](mailto:iblank@psych.ucla.edu)

### CRediT Author Statement

| Role | Contributors |
|------|-------------|
| Conceptualization | David G. Kamper, Idan Blank |
| Methodology | David G. Kamper, Idan Blank |
| Software | David G. Kamper |
| Formal Analysis | David G. Kamper |
| Investigation | David G. Kamper, Anna Walburger |
| Data Curation | David G. Kamper, Anna Walburger |
| Writing — Original Draft | David G. Kamper |
| Writing — Review & Editing | David G. Kamper, Idan Blank |
| Visualization | David G. Kamper |
| Supervision | Idan Blank |
| Project Administration | David G. Kamper |

## License

This repository is intended for academic research purposes. Please contact the authors before reusing data or materials.

## Citation

If you use these materials, please cite:

> Kamper, D. G., & Blank, I. (2025). An Empirical Analysis of Laypersons' Interpretation of Second Amendment Structure. Manuscript in preparation, University of California, Los Angeles.
