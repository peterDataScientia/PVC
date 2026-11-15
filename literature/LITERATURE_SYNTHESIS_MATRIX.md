# Thermal Degradation Kinetics and Lifetime Prediction of Perovskite Solar Cells

**Focused literature synthesis and research gap**  
**Date:** 15 November 2026  
**Basis:** Selected studies on operational ageing, thermally accelerated degradation and lifetime modeling.

## Critical literature synthesis

The increasing power conversion efficiency of perovskite solar cells has intensified interest in whether these devices can maintain their performance during sustained operation. Jacobsson et al. (2022) assembled more than 42,400 published device records, demonstrating the breadth of research on perovskite composition, architecture and photovoltaic performance. However, the stability evidence reported across studies is less directly comparable because devices are tested under different illumination, temperature and operating conditions. Hartono et al. (2023) moved beyond individual performance measurements by analyzing 2,245 maximum-power-point-tracking ageing trajectories over a standardized 150-hour period. They identified distinct patterns of efficiency evolution and reported an association between initial efficiency and short-term stability. Together, these studies show why high initial efficiency and operational durability should be evaluated separately: device performance at the start of testing does not establish either the rate of subsequent deterioration or the time required to reach a defined failure threshold.

Temperature-dependent experiments provide a physical basis for estimating how rapidly photovoltaic performance changes under accelerated stress. A 2024 investigation of flexible MAPbI₃ modules used thermal exposure at 85, 95 and 105 °C and reported an apparent activation energy of 1.062 eV for maximum-output degradation. The study also identified differences in the temporal behavior of electrical-performance parameters, indicating that a single degradation rate need not describe every aspect of device deterioration. Research on stabilized self-assembled interfacial layers reported in *Nature Energy* (2025 volume) further demonstrated that thermal robustness can be altered through device design. These findings establish the usefulness of thermally accelerated measurements while also limiting their interpretation. An activation energy derived from one architecture, electrical endpoint or temperature interval cannot automatically represent another system. The physical relevance of Arrhenius analysis therefore depends on whether the measured degradation can be described consistently within the investigated experimental regime.

Computational studies have extended stability analysis from kinetic characterization to prediction. Alsulami et al. (2024) modeled perovskite stability using 6,038 records and reported different model correlations for an architecture-specific subset and a pooled dataset, indicating that the structure of the experimental population can affect the relationships recovered by a predictive model. Dunlap-Shohl et al. (2024) investigated T80 prediction using physicochemical information from 45 ageing experiments on CH₃NH₃PbI₃-based devices, establishing a direct precedent for estimating lifetime from early degradation measurements. Nevertheless, stability modeling and lifetime forecasting do not have identical requirements. A model may reproduce changes already observed in an efficiency trajectory without accurately estimating when an independently tested device will reach 80% of its initial performance. Differences in device architecture, observation time and validation design also prevent prediction statistics from separate studies from being interpreted as a controlled comparison of kinetic models.

Collectively, the literature shows that degradation patterns are heterogeneous, temperature can accelerate performance loss, and model-based lifetime estimation is feasible under particular experimental conditions. What remains important is determining how reliably kinetic descriptions of measured degradation support subsequent predictions. This study therefore examines thermal degradation rates and T80 estimates using temperature-resolved experimental ageing trajectories, with attention to kinetic formulation, measurement duration and independent-sample validation. The investigation does not assume that improved curve fitting necessarily produces accurate lifetime estimates. Instead, it evaluates the extent to which the information contained in accelerated ageing measurements can support physically interpretable and testable predictions of photovoltaic durability.

## Interconnected limitations identified in the reviewed studies

| Evidence-based limitation | Specific precedent | Implication for the present investigation |
|---|---|---|
| High initial performance does not establish operational stability | Jacobsson et al. (2022); Hartono et al. (2023) | Analyze time-dependent efficiency retention rather than using initial PCE as a lifetime surrogate. |
| Heterogeneous degradation trajectories | Hartono et al. (2023), 2,245 ageing curves | Evaluate competing kinetic forms instead of assuming one universal decay shape. |
| Dependence of apparent kinetic parameters on experimental conditions | Flexible MAPbI₃ module study (2024), 85–105 °C | Compare rates within defined temperature ranges, endpoints and observation windows. |
| Influence of device architecture on thermal response | Self-assembled interfacial-layer study (2025 volume); Alsulami et al. (2024) | Account for sample and device-system differences before interpreting pooled estimates. |
| Limited comparability of predictive performance between studies | Alsulami et al. (2024); Dunlap-Shohl et al. (2024) | Compare models under common validation conditions and distinguish degradation prediction from T80 prediction. |
| Restricted evidence for transfer of early-ageing predictions | Hartono et al. (2023), 150-hour trajectories; Dunlap-Shohl et al. (2024), 45 experiments | Evaluate future threshold prediction directly and report unobserved or non-estimable T80 outcomes. |

## Focused unresolved research question

To what extent can temperature-dependent degradation models describe the ageing kinetics of perovskite solar cells and predict T80 under independent experimental evaluation?

## Interpretation boundaries

- An apparent activation energy characterizes the chosen kinetic model and measurement regime; it does not establish a unique microscopic degradation mechanism.
- A good fit to measured PCE trajectories does not demonstrate accurate future T80 prediction.
- Multiple pixels from one sample should not automatically be treated as independent devices.
- Extrapolated lifetime estimates must be distinguished from observed T80 events.
- The reviewed papers establish precedents for Arrhenius analysis and T80 prediction; the contribution lies in the evaluation of their reliability under the selected conditions.

## Core study references

- Jacobsson et al. (2022), *Nature Energy*. https://doi.org/10.1038/s41560-021-00941-3
- Hartono et al. (2023), *Nature Communications*. https://doi.org/10.1038/s41467-023-40585-3
- Alsulami et al. (2024), *Journal of Materials Chemistry A*. https://doi.org/10.1039/D3TA05966A
- Dunlap-Shohl et al. (2024), *Journal of Materials Chemistry A*. https://doi.org/10.1039/D3TA06668A
- Flexible MAPbI₃ module thermal-stability study (2024), *Solar Energy Materials and Solar Cells*. https://doi.org/10.1016/j.solmat.2024.113148
- Self-assembled bilayer stability study (2025 volume), *Nature Energy*. https://doi.org/10.1038/s41560-024-01689-2
