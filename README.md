# Megacarcasses-woodies

This repository contains the R scripts, processed datasets, figures, and supporting files used for analyses presented in the dissertation chapter and manuscript examining how African savanna elephant megacarcasses influence woody vegetation structure, foliar chemistry, leaf traits, browse dynamics, soil resistance, and seedling recruitment in Kruger National Park, South Africa.

The project investigates how long-lasting elephant cadaver decomposition islands (CDIs) restructure savanna vegetation through localized nutrient enrichment and physical disturbance. Analyses focus on spatial and temporal patterns in soil nutrients, foliar isotopes and chemistry, woody leaf traits, browsing pressure, and woody seedling establishment across carcass age gradients and contrasting basalt and granite soil systems.

## Repository contents

* `code_woody_all_v3.qmd` — Primary Quarto workflow used for data processing, statistical analyses, model selection, and figure generation.
* `data/` — Processed datasets used in analyses, including foliar chemistry, leaf traits, browse, seedling, and soil resistance datasets.
* `figures/` — Output figures generated for manuscript preparation.
* `tables/` — Supplemental tables including model selection outputs and coefficient summaries.
* `supplemental/` — Additional supporting material and exported outputs.

## Analytical overview

Analyses were conducted in R using generalized linear mixed models (GLMMs) implemented primarily through `glmmTMB`, with model diagnostics evaluated using `DHARMa`. Candidate models evaluated the effects of:

* distance from CDI center,
* soil type,
* carcass age,
* sampling year,
* and their interactions,

while accounting for repeated sampling structure using random intercepts for site.

Model families included Gamma (log link), Gaussian, and binomial-logit formulations depending on response structure and diagnostic performance.

## Study system

Field data were collected across elephant megacarcass sites distributed throughout Kruger National Park, South Africa, spanning carcasses ranging from recent mortality events to sites more than seven years postmortem. Sampling incorporated both carcass and paired matrix/control locations across multiple years.

## Reproducibility

All analyses and figure-generation workflows are contained within the repository to support transparency and reproducibility. Paths may need minor adjustment depending on local directory structure.

## Author

Ryan Helcoski
Department of Wildland Resources
Utah State University

Collaborative contributions and manuscript coauthors are acknowledged within associated manuscripts and supplemental materials.
