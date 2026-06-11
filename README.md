# Megacarcasses-woodies

Code and processed datasets associated with analyses of elephant megacarcass effects on woody vegetation, browse dynamics, foliar chemistry, leaf traits, soil resistance, and seedling recruitment in Kruger National Park, South Africa.

## Repository contents

### Analysis workflow

* `code_woody_all_publication.qmd`
  Main Quarto workflow used for data processing, statistical analyses, model selection, and figure generation.

### raw datasets

* `soil_leaf_chem.csv` — Soil and foliar chemistry data
* `leaf_traits.csv` — Woody leaf trait measurements
* `vert_browse.csv` — Woody browse survey data
* `soil_resistance.csv` — Soil penetration resistance data
* `seedlings.csv` — Woody seedling survey data

### Model outputs

* `model_selection_and_coefficients.xlsx`
  Candidate model rankings, ΔAICc values, Akaike weights, parameter estimates, and model summaries for all primary response variables.

## Study overview

This project examines how African savanna elephant megacarcasses function as long-lasting cadaver decomposition islands (CDIs) that restructure local nutrient dynamics, woody vegetation responses, browsing pressure, and seedling recruitment across spatial and temporal gradients.

Fieldwork was conducted in Kruger National Park, South Africa, across carcass sites spanning a multi-year postmortem age gradient and contrasting basalt and granite soil systems.

## Analytical approach

Analyses were conducted in R using generalized linear mixed models (GLMMs), primarily implemented through `glmmTMB`. Candidate models evaluated the effects of:

* distance from carcass center,
* soil type,
* years postmortem,
* and sampling year,

with site included as a random effect where appropriate.

Model diagnostics were evaluated using `DHARMa`, and model selection was conducted using AICc-based approaches.

## Reproducibility

The repository is intended to support analytical transparency and reproducibility. Some file paths may require adjustment depending on local directory structure.

## Author

Ryan Helcoski
Department of Wildland Resources
Utah State University

## Acknowledgments

We thank South African National Parks (SANParks), collaborating researchers, and field assistants who supported field sampling and logistics associated with this project.
