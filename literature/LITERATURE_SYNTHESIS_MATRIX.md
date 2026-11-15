# Thermal Degradation Kinetics and Lifetime Prediction of Perovskite Solar Cells

## Critical literature synthesis

Perovskite solar cells have achieved substantial advances in power conversion efficiency, bringing operational stability into sharper focus as a determinant of practical photovoltaic performance. Jacobsson et al. (2022) compiled more than 42,400 published device records, establishing a broad basis for examining relationships among composition, architecture, fabrication and efficiency. The challenge of interpreting stability across different experimental conditions was subsequently addressed from a time-resolved perspective by Hartono et al. (2023), who examined 2,245 maximum-power-point-tracking (MPPT) ageing trajectories over 150 hours. Their analysis identified distinct patterns of efficiency evolution and an association between initial efficiency and short-term stability. These investigations demonstrate the complementary roles of large-scale device characterization and longitudinal monitoring: the former describes variation across photovoltaic systems, whereas the latter reveals how their performance evolves during operation. Establishing the rate of that evolution, however, requires a kinetic description of the observed efficiency changes.

Accelerated thermal experiments provide a means of quantifying the temperature dependence of degradation. A 2024 study of flexible MAPbI₃ modules examined performance at 85, 95 and 105 °C and reported an apparent activation energy of 1.062 eV for maximum-output degradation using Arrhenius analysis. Differences in the temporal responses of individual electrical parameters also indicated that degradation was not represented equally by every performance measure. Related research on stabilized self-assembled interfacial layers, reported in *Nature Energy* (2025 volume), showed that modifying device interfaces improved thermal robustness. Considered together, these findings connect degradation kinetics to both thermal stress and device design. The resulting apparent rate parameters characterize the tested electrical endpoint, temperature interval and architecture. This dependence is particularly relevant when comparing efficiency-loss trajectories across different perovskite systems, where changes in measured degradation rates reflect the combined influence of operating conditions and material structure.

Computational investigations have extended these measurements toward predictive stability assessment. Alsulami et al. (2024) analyzed 6,038 records using sequential minimal optimization regression and reported correlations of 0.963 for a p–i–n device subset and 0.699 for a pooled architecture analysis in the reported training evaluations. This contrast illustrates the influence of device-population heterogeneity on fitted relationships. Dunlap-Shohl et al. (2024) approached prediction through a different endpoint, combining physicochemical information with machine learning to estimate T80 using 45 degradation experiments involving CH₃NH₃PbI₃-based devices. Whereas stability regression quantifies relationships between measured characteristics and performance, T80 prediction seeks to estimate the future time at which performance reaches a defined fraction of its reference value. The distinction has practical consequences: reproducing measured efficiency changes and forecasting a future threshold crossing require different evaluation criteria. Model comparisons are therefore most informative when the prediction endpoint, experimental grouping and held-out observations are specified consistently.

The reviewed evidence establishes substantial progress in identifying degradation patterns, describing thermal acceleration and estimating photovoltaic lifetime. It also highlights the need to examine how kinetic assumptions influence the interpretation of accelerated ageing and the accuracy of subsequent predictions. The present investigation evaluates temperature-dependent MPPT efficiency trajectories using linear, exponential and stretched-exponential descriptions, with Arrhenius analysis of apparent degradation rates and independent-sample evaluation of T80 prediction. By examining kinetic behaviour and lifetime prediction within the same experimental framework, the study connects physical characterization of performance loss with the practical assessment of photovoltaic durability.

## Interconnected limitations identified in the reviewed studies

| Evidence-based limitation | Specific precedent | Implication for the study |
|---|---|---|
| Variation in operational ageing patterns | Hartono et al. (2023), 2,245 MPPT trajectories | Compare alternative kinetic descriptions of measured efficiency retention. |
| Dependence of thermal rate estimates on electrical endpoint and test conditions | Flexible MAPbI₃ module study (2024), 85–105 °C | Estimate apparent kinetic parameters within specified temperature intervals and observation windows. |
| Device architecture influences stability response | Self-assembled interfacial-layer study (2025 volume); Alsulami et al. (2024) | Account for device systems and related samples when comparing degradation behaviour. |
| Predictive statistics differ with the modeled outcome and data composition | Alsulami et al. (2024); Dunlap-Shohl et al. (2024) | Evaluate PCE-trajectory prediction and T80 prediction as distinct outcomes under explicit validation procedures. |
| Restricted observation periods in ageing studies | Hartono et al. (2023), 150-hour trajectories | Distinguish observed threshold crossings from extrapolated lifetime estimates and incomplete follow-up. |

## Focused unresolved research question

To what extent can temperature-dependent kinetic models describe the degradation of perovskite solar cells and predict T80 under independent experimental evaluation?

## Core study references

- Jacobsson et al. (2022), *Nature Energy*. https://doi.org/10.1038/s41560-021-00941-3
- Hartono et al. (2023), *Nature Communications*. https://doi.org/10.1038/s41467-023-40585-3
- Alsulami et al. (2024), *Journal of Materials Chemistry A*. https://doi.org/10.1039/D3TA05966A
- Dunlap-Shohl et al. (2024), *Journal of Materials Chemistry A*. https://doi.org/10.1039/D3TA06668A
- Flexible MAPbI₃ module thermal-stability study (2024), *Solar Energy Materials and Solar Cells*. https://doi.org/10.1016/j.solmat.2024.113148
- Self-assembled bilayer stability study (2025 volume), *Nature Energy*. https://doi.org/10.1038/s41560-024-01689-2
