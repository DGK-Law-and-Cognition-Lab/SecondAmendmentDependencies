# Second Amendment Dependencies

This repository contains materials for the project **"An Empirical Analysis of Laypersons’ Interpretation of Second Amendment Structure"** by David G. Kamper, Anna Walburger, and Idan Blank (UCLA).
The project empirically investigates how laypersons interpret the syntactic dependencies of the Second Amendment, with implications for constitutional theory and judicial practice.

## Table of Contents

* [Introduction](#introduction)
* [Preregistrations](#preregistrations)
* [Repository Structure](#repository-structure)
* [Key Materials](#key-materials)
* [How to Run Analyses](#how-to-run-analyses)
* [Contact](#contact)

---

## Introduction

The linguistic structure of the Second Amendment has posed persistent interpretive challenges, especially for textualist and originalist constitutional theories. This project presents the first systematic empirical investigation of how contemporary laypersons interpret sentences mirroring the Amendment’s structure, using neutral topics to isolate linguistic processing from political attitudes.

---

## Preregistrations

---

## Repository Structure

```
.
├── Code/
│   └── R/
│       └── Pilot/
│           ├── PilotAnalysis_V3.Rmd
│           └── PilotAnalysis_V3.html
├── Data/
│   ├── Cleaned_Numeric_Second Amendment Dependencies_Pilot.csv
│   ├── Cleaned_Response_Second Amendment Dependencies_Pilot.csv
│   └── q1_rewrite_responses_for_coding_edited.csv
├── Docs/
├── Figures/
├── Experiment/
│   ├── Qualtrics.pdf
```

---

## Key Materials

* **Data:**

  * [Cleaned Numeric Data (CSV)](./Data/Cleaned_Numeric_Second%20Amendment%20Dependencies_Pilot.csv)
  * [Cleaned Response Data (CSV)](./Data/Cleaned_Response_Second%20Amendment%20Dependencies_Pilot.csv)
  * [Coded Q1 Rewrites (CSV)](./Data/q1_rewrite_responses_for_coding_edited.csv)

* **Code:**

  * [Pilot Analysis RMarkdown](./Code/R/Pilot/PilotAnalysis_V3.Rmd)
  * [Pilot Analysis HTML Output](.https://dgk-law-and-cognition-lab.github.io/SecondAmendmentDependencies/Code/R/Pilot/PilotAnalysis_V3.html)

* **Experiment Materials:**

  * [Qualtrics Survey (PDF)](.https://dgk-law-and-cognition-lab.github.io/SecondAmendmentDependencies/Experiment/Qualtrics.pdf)

---

## How to Run Analyses

1. **Requirements:**

   * R (recommended ≥ 4.0)
   * R packages: `tidyverse`, `lme4`, `ordinal`, (and others as specified in the RMarkdown)

2. **Running Analyses:**

   * Open [PilotAnalysis\_V3.Rmd](./Code/R/Pilot/PilotAnalysis_V3.Rmd) in RStudio or your preferred IDE.
   * Ensure the data files in `/Data/` are present.
   * Knit to HTML or run code chunks as needed.
   * Results and figures will be saved to `/Figures/` if the script generates output.

3. **Viewing Results:**

   * See summary outputs in [PilotAnalysis\_V3.html](.https://dgk-law-and-cognition-lab.github.io/SecondAmendmentDependencies/Code/R/Pilot/PilotAnalysis_V3.html).

---

## Contact

**Lead Author:**
David G. Kamper
Department of Psychology, UCLA
Email: [davidgkamper@ucla.edu](mailto:davidgkamper@ucla.edu)
Website: [dgkamper.github.io](https://dgkamper.github.io)

---

## License

(MIT)

---

**[Back to top](#second-amendment-dependencies)**
