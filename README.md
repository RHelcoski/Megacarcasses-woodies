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

Funding for this research was provided by the U.S. National Science Foundation (DEB 2128092, 2128093, 2128094), Utah State University, the South African National Research Foundation (PDP/2022/03/15/09), The American Philosophical Society, The Explorers Club, Fjällräven, The US Fulbright Program, The African Safari Club of Florida, and the Kosciuszko Foundation. Additionally, we thank the South African Environmental Observation Network (NRF-SAEON) for financial, logistical, and administrative support. Research was completed under permits from South African National Parks (SS554, and SS1171). We thank SANParks for their support of this research, particularly Sandra Snelling and section rangers for providing locations and ages of carcasses, game guards (Siza Desmond Mabaso, Isaac Sedibe, Velly Ndlovu, Herman Honest Ntimane, Anoint Mashele, Amanda Mashiane, Khensani Mkhonto, Martin Sarela) for providing guidance and protection in the field, and Mmathapelo Fumo for providing laboratory support at Kruger. We thank Mr. Lucky Sithole (Cedara Analytical Services Laboratory), Ms. Terina Vermeulen (Eco-Analytica Laboratory), and Dr. Janine Colling (BIOGRIP laboratory) for their laboratory support. Select data used in this research paper were generated using equipment in the DSI-funded BIOGRIP soil and water node at Stellenbosch University. Finally, we thank our research assistants and field technicians from the Good Works Foundation (GWF), Kruger National Park and South Africa National Parks’ Work Integrated Learning (WIL) Programme; Ally Mahori, Charmaine J. Malaza, Mirandah Mnisi, Natatia Nyalungu, Busisiwe Masilela, Theocracy Mukansi, Genesis Boitelo Faer, Lucy Masego Madiba, Gladden Green, Octavia Mondli Ngomane, Real Njabulo Mhlanga, Sabelo Collen Mahlangu, Mandisa Ntombizethu Khumalo, Gillian Ntsako Ngobeni, Mushavhela Andani Patient, Amaze Khoza, Lorraine Molema, Connie Jiyane, Erwin Ngomane, Mandla Masela, Sbusiso Chagwe, Nancy Banda, Nxumalo Nomthandazo, Dzunani Nzobe, Matlawa Lebogang, and Mosiya Thandiwe, Ngcobo Yenama, Shabangu Shirley, and Sibusiso Mnisi.
