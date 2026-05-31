---
aliases:
- collaboration
author: Smitom Borah
date: "2024-02-02"
description: Research works by Smitom
title: My research
---

## Current Projects

### Identification of Priority Lakes and Watersheds for Nutrient Intervention in the U.S.
*(Feb 2026 – present)*

Developing comprehensive datasets on waterbody and watershed characteristics through compilation and imputation. Constructing a preliminary prioritization framework for nutrient management interventions across the United States.

---

### Ensemble Response Curves of Harmful Algal Blooms and Hypoxia in Lake Erie
*(Aug 2025 – Feb 2026)*

Explored management implications for HABs and hypoxia mitigation through ensemble response curves. Developed a multi-model ensemble framework to characterize nutrient load-response relationships in aquatic systems.

---

## PhD Research

### Riverine Phosphorus Losses Across the U.S.
*(Jan 2024 – Jul 2025)*

Investigated hydrometeorological drivers of phosphorus export across US watersheds using hierarchical Bayesian modeling. Explored the influence of climate and land management factors on watershed phosphorus losses at a national scale.

---

### Internal Phosphorus Loading in Large U.S. Lakes
*(Jul 2022 – Jul 2024)*

When lakes receive too much phosphorus from surrounding watersheds, managers often respond by reducing external inputs: cutting fertilizer runoff, upgrading wastewater treatment, and similar measures. But even after external loads drop, many lakes stubbornly remain polluted for years or even decades. A key reason is internal phosphorus loading (IPL), which refers to phosphorus that has accumulated in lake sediments over time and is released back into the water column under warm, oxygen-depleted (anoxic) conditions every summer. Despite its importance, IPL had never been systematically estimated across the entire contiguous United States, largely because the field measurements needed are expensive, labor-intensive, and available for only a handful of lakes.

In this project, I developed a hybrid machine learning and statistical modeling framework to estimate summer sediment phosphorus release rates (SRRs) for 5,899 large lakes and reservoirs across the contiguous US. The framework chained two random forest models (one predicting bottom-water temperature and one predicting surface-water total phosphorus) into a mixed-effects regression model for SRR, with full uncertainty propagation through the linked models. Drawing on national datasets for water quality, land use, lake morphometry, and climate, the framework produced the first comprehensive, uncertainty-quantified map of summer IPL across the US.

{{< figure src="/images/ipl_abstract_graphic.png" alt="Hybrid modeling framework and predicted summer sediment phosphorus release rates across the contiguous US" caption="Hybrid modeling framework (left) combining random forest and mixed-effects regression models, and the resulting predicted summer sediment phosphorus release rates across the contiguous US (right). Figure from: Borah et al. (2025), Environmental Science & Technology. https://doi.org/10.1021/acs.est.4c13431" width="75%" >}}

**Key findings:**

- Summer sediment phosphorus release rates range from 1 to 37 mg/m²/day across US lakes, with nearly one-third of lakes exceeding 10 mg/m²/day. The highest rates are concentrated in agricultural regions of the Plains and Midwest, where surface-water phosphorus concentrations are already elevated.
- In relatively dry summers, when external loading is low, internal phosphorus loading is estimated to exceed watershed-level external loading in 26% of US watersheds. This underscores that IPL can actively undermine external nutrient management efforts and delay water quality recovery by decades.
- The study introduces a novel approach to propagate uncertainty from random forest models through linked statistical models, showing that the majority of prediction uncertainty (about 65%) originates from the machine learning inputs rather than the regression model itself. This is a methodological contribution applicable beyond water quality research.

---

### Bayesian Reservoir Modeling, Jordan Lake, NC
*(Jan 2021 – Dec 2022)*

Jordan Lake is a drinking water reservoir outside of Raleigh, NC, that has struggled with eutrophication since its impoundment in 1983. Despite decades of efforts to reduce nutrient runoff from surrounding watersheds, water quality improvements have been slow and uneven across the reservoir. A key but poorly understood culprit is internal phosphorus loading (IPL): phosphorus accumulated in the lake sediments over decades that gets released back into the water column each summer under warm, low-oxygen conditions. Estimating IPL is notoriously difficult because it requires either costly field experiments or complex models that demand data rarely available for most waterbodies.

In this project, I developed a novel modeling framework that estimates IPL dynamics by combining a segmented mass-balance phosphorus model with long-term surface-water monitoring data and Bayesian statistical inference. The reservoir was divided into four spatial segments to capture longitudinal gradients in water quality, and the model was calibrated against nearly four decades (1983 to 2018) of observations. A random forest sub-model was used to account for seasonal thermal stratification, linking bottom-water temperature to surface phosphorus concentrations. The Bayesian framework allowed systematic estimation of nutrient cycling rates, including sediment recycling, burial, and settling, along with full uncertainty quantification. The calibrated model was then used to project future phosphorus dynamics under climate warming scenarios and to evaluate the long-term effectiveness of different management interventions, including external load reductions, sediment capping, and sediment dredging.

{{< figure src="/images/jl_bayesian_fig3.png" alt="Time series of simulated and observed total phosphorus in Jordan Lake segments" caption="Time series of monthly simulated (line) and observed (dots) total phosphorus concentrations in the water column and sediment layer across four segments of Jordan Lake (1983 to 2018), with 90% prediction intervals. Figure 3 from: Borah et al. (2025), Journal of Environmental Management. CC BY 4.0. https://doi.org/10.1016/j.jenvman.2025.125538" width="75%" >}}

**Key findings:**

- Internal phosphorus loading in Jordan Lake has become the dominant summer phosphorus source, contributing nearly twice the external load during summer months (0.53 g/m²/month). Even as watershed inputs declined by 44% over the study period, IPL remained relatively stable, explaining why surface phosphorus concentrations dropped by only 36% in response.
- While rising temperatures are projected to intensify both phosphorus release from and deposition back to the sediments, these competing effects nearly cancel out for Jordan Lake, resulting in little net change in water-column phosphorus concentrations over the next 70 years. This contrasts with more northern lakes and suggests that recovery in Jordan Lake will be driven more by management than by climate.
- Simulations of management scenarios show that reducing external loads alone will take roughly 62 years to achieve substantial water quality improvements, while in-lake interventions such as sediment capping or dredging can deliver faster but less sustained benefits. A combined strategy targeting both internal and external loading is projected to produce the most immediate and durable improvements.

---

## Prior Research

### Water Quality Dynamics in Deepor Beel, India
*(Aug 2017 – Jun 2019)*

Experimental measurement of nutrients in water, plants, and sediment samples from 23 sampling stations in Deepor Beel (a Ramsar site) over approximately 1.5 years. Developed a one-dimensional ecological model to understand nitrogen and phosphorus dynamics and assess eutrophication levels.

---

### Assessment of Heavy Metal Contamination in Deepor Beel, India

Experimental measurement of 7 heavy metals (Mg, Cr, Cd, Fe, Mn, Cu, and Pb) in water, plants, sediment, and fish samples from Deepor Beel (a Ramsar site).

---
