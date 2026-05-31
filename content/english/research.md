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

### Riverine Phosphorus Losses Across the U.S. <span class="badge-prep">(Manuscript in preparation)</span>
*(Jan 2024 – Jul 2025)*

Phosphorus lost from watersheds to rivers and streams is a leading cause of eutrophication in downstream lakes and coastal waters. While it is well established that precipitation drives much of this export through surface runoff, two important questions have remained largely unresolved at the national scale: which representation of precipitation best captures phosphorus export dynamics, and how does temperature factor into the picture? Total annual precipitation is the most commonly used metric in large-scale phosphorus models, but it blurs together the water that actually runs off and the water lost to evapotranspiration, which never reaches streams. Meanwhile, the role of temperature in regulating phosphorus export across the contiguous US has received little systematic attention.

In this project, I developed a hierarchical Bayesian modeling framework to systematically evaluate different representations of precipitation and temperature as drivers of annual total phosphorus (TP) export across 131 watersheds spanning the contiguous US from 2002 to 2012. The model was built on a hybrid structure that accounts for multiple phosphorus sources, including agricultural inputs, urban waste, and background geogenic soil phosphorus, along with waterbody retention. Using this framework, I tested ten model versions with different combinations of total, net (precipitation minus actual evapotranspiration), and extreme precipitation, as well as temperature. For the best-performing model, I applied Shapley value analysis to quantify and map each predictor's contribution to phosphorus export across the country, representing the first application of this method within a parametric water-quality model.

**Key findings:**

- Net precipitation (total precipitation minus actual evapotranspiration) outperforms total precipitation as a predictor of phosphorus export, particularly for capturing intra-regional variability. When combined with an extreme precipitation term, it produces the best overall model performance, as extreme events capture episodic flushing dynamics that net precipitation alone cannot fully represent.
- Temperature has an overall inverse relationship with phosphorus export at the national scale, acting primarily through evapotranspiration: warmer conditions reduce the water available for runoff, limiting phosphorus mobilization. This suggests that in a warming climate, the effect of temperature on phosphorus export will depend heavily on how precipitation patterns also shift.
- Shapley value analysis reveals that precipitation is the dominant driver of both spatial and interannual variability in phosphorus exports, emerging as the primary factor in 64% of watersheds across the US. Agricultural inputs are the primary driver in another 18% of watersheds, concentrated in the Midwest and Mid-Atlantic, while background soil phosphorus dominates in much of the western US where natural geogenic sources are high but precipitation is low.

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

Deepor Beel is a Ramsar-designated wetland in the heart of Guwahati city, Assam, India, and one of the most ecologically significant freshwater bodies in the region. Despite its protected status, the wetland has faced severe and worsening eutrophication driven by agricultural runoff, municipal wastewater, leachate from a nearby landfill, industrial activity, and encroachment. The sediment column of the wetland has simultaneously become a repository for heavy metals from these same sources, raising additional concerns about bioaccumulation and long-term ecological risk. Restoring Deepor Beel requires understanding not just the current state of its water quality, but the underlying nutrient cycling and contamination processes that sustain and amplify degradation over time.

As part of this collaborative project at IIT Guwahati, I contributed to an intensive 17-month field sampling campaign across 23 stations in the wetland, collecting water, sediment, and water hyacinth samples for analysis of nitrogen, phosphorus, and seven heavy metals (Cr, Cd, Fe, Mn, Cu, Pb, and Mg). This dataset supported two separate studies. The first developed a one-dimensional ecological model in MATLAB simulating nutrient cycling across the water column, sediment, and plant layers, tracking eight state variables through calibration, validation, and scenario testing. The model was used to evaluate two management options: harvesting water hyacinths and installing a nutrient treatment unit at the wetland inlet. The second study assessed heavy metal contamination and ecological risk through hierarchical cluster analysis, principal component analysis, and a suite of contamination indices (contamination factor, pollution load index, enrichment factor, and geo-accumulation index), complemented by chemical speciation analysis to determine the forms in which each metal persists in the sediment column.

**Key findings:**

- The ecological model successfully reproduced observed nutrient dynamics across all eight state variables (validation R² of 0.63 to 0.99), and showed that harvesting water hyacinths is ineffective for long-term eutrophication control. Because plant nutrient uptake and decay rates are low relative to loading and cycling rates in the water column, removing plants does little to reduce the nutrient pool. Installing a treatment unit at the wetland inlet, by contrast, is projected to substantially and durably reduce nutrient concentrations across all compartments.
- Heavy metal contamination is spatially structured by pollution sources: sites near the Boragaon landfill showed the highest contamination, followed by the industrial zone, with the central wetland least affected. Contamination is most pronounced in the post-monsoon season, when reduced turbulence and receding water levels facilitate the settling of metals from the water column to the sediment. Monsoon dilution keeps contamination levels low during the wet season.
- Chemical speciation analysis revealed that cadmium is the dominant ecological risk driver, primarily present in readily exchangeable and reducible forms that make it highly mobile and bioavailable. While overall contamination indices remain in the moderate range, the combination of multiple active pollution sources and the wetland's declining area signals that without prompt intervention, contamination could escalate to irreversible levels.

---
