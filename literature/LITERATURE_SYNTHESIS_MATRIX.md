# Literature Synthesis Matrix
## Thermal Degradation Kinetics and Lifetime Prediction of Perovskite Solar Cells

**Evidence review date:** 15 November 2026. This is a critical synthesis: the last column explicitly identifies *our appraisal or testable opportunity*, not necessarily a limitation explicitly acknowledged by the original authors. Do not treat dataset records, manuscripts, and peer-reviewed research articles as the same evidence category.

## Table 1. Study-by-study evidence matrix

| # | Study / source | Study objective and evidence | Methods / data | Main findings reported by authors | Critical appraisal and relevance to this research |
|---|---|---|---|---|---|
| 1 | **Jacobsson et al. (2022), Nature Energy** — [DOI](https://doi.org/10.1038/s41560-021-00941-3) | Build a FAIR-oriented open database of published perovskite devices | Literature-derived device database: **over 42,400 devices**, up to **100 parameters** | Demonstrates potential of systematic device metadata and large-scale analysis | Heterogeneous study conditions and missing endpoint information limit direct kinetic inference; useful for background and data provenance, not a replacement for matched ageing traces |
| 2 | **Hartono et al. (2023), Nature Communications** — [DOI](https://doi.org/10.1038/s41467-023-40585-3) | Relate operational PCE to stability and ageing-curve patterns | **2,245** MPPT ageing traces; standardized to **150 hours**; statistics and self-organizing map clustering | Higher maximum PCE associated statistically with improved short-term stability; ageing curves cluster into recurring shapes | This is an important *precedent*, not an unresolved question by itself. The public processed PKL contains MPPT traces but does not directly expose per-curve temperature/architecture mapping; a short fixed window limits long-horizon T80 generalization |
| 3 | **Alsulami et al. (2024), Journal of Materials Chemistry A** — [DOI](https://doi.org/10.1039/D3TA05966A) | Model device stability across materials and architectures | **6,038** database records; sequential minimal optimization regression (SMOreg); architecture-specific subsets | Training correlation reported as **0.963** in p–i–n subset versus **0.699** overall | These are reported training correlations, not proof of cross-study performance. For our work, device grouping and leakage-aware independent testing are essential |
| 4 | **Dunlap-Shohl et al. (2024), Journal of Materials Chemistry A** — [DOI](https://doi.org/10.1039/D3TA06668A) | Predict T80 from early degradation dynamics, ambient factors, and physicochemical features | **45** degradation experiments on CH3NH3PbI3 device stack; hybrid physicochemical ML; held-out samples | Authors report approximately **40% average T80 prediction accuracy** on unseen samples; a kinetics-informed feature was important | Direct precedent for lifetime prediction. Small, composition-specific experimental scope motivates careful examination of transferability, model uncertainty and comparability of T80 event definitions |
| 5 | **Thermal stability test on flexible perovskite solar cell modules (2024), Solar Energy Materials and Solar Cells** — [DOI](https://doi.org/10.1016/j.solmat.2024.113148) | Determine thermal stability and apparent activation energy of flexible MAPbI3 modules | Heating at **85, 95 and 105 °C** for extended periods; periodic electrical tests; Arrhenius extrapolation | Reported **1.062 eV** apparent activation energy for maximum output; some electrical characteristics exhibited multiple degradation stages | A direct Arrhenius precedent. The reported activation energy is device/system- and endpoint-specific, so it should not be directly compared as though identical to an MPPT-derived constant at 25–65 °C |
| 6 | **Dong et al. (2025), Nature Energy** — [DOI](https://doi.org/10.1038/s41560-024-01689-2) | Improve heat tolerance of perovskite cells by stabilizing SAM interfaces | Experimental comparison of SAM and covalently interconnected self-assembled bilayer devices under heat, damp heat and thermal cycling | Bilayer enhanced thermal robustness; champion devices reported low PCE loss under long accelerated tests | Demonstrates that architecture/interface design changes thermal response; warns against pooling unlike material stacks as if they share one degradation mechanism |
| 7 | **Hartono et al. (2026), Accelerated Perovskite Solar Cells Ageing Dataset v2** — [Zenodo DOI](https://doi.org/10.5281/zenodo.21242242) | Publish experimental temperature-dependent ageing measurements for SAM-based devices | CSV archive `dataset_SAM.zip` with time-varying MPPT PCE at multiple temperatures; authors link processing code | Provides experimental trajectories for independent reanalysis; **this is a dataset record, not itself a peer-reviewed comparative modeling result** | Direct source for this project's temperature-dependent kinetics. Must audit time gaps, baseline definition, device/pixel grouping, uneven observation durations and true versus interval-censored T80 |
| 8 | **Parion & Vermang (2026), wide-bandgap perovskite degradation dataset** — [Zenodo](https://zenodo.org/records/18423433) | Document stress-dependent degradation in scalable wide-bandgap devices | ISOS-L1 light stress, ISOS-D2 heat/storage, ISOS-L2 light plus heat; 1.68 eV and reference devices | Dataset description reports more rapid deterioration under thermal and combined stress than light alone | Evidence of stress-dependent pathways; non-equivalent protocols and device designs prevent unqualified numerical pooling with the primary datasets |
| 9 | **Erdil et al. (2026), accelerated ion-migration ageing article record** — [Zenodo](https://zenodo.org/records/21022057) | Compare forward-bias/dark-recovery ageing dynamics with field operation | Bias ageing and recovery; comparison to outdoor operation over about **20 months** | Reported partly recoverable performance changes linked to ion migration and stress conditions | Critical relevance: reversible performance shifts can resemble a threshold crossing, so sustained T80 detection should check recovery |
| 10 | **Peng & Kyaw (2026), stability-prediction evidence-pipeline benchmark** — [Zenodo](https://zenodo.org/records/22158454) | Assess dependence of literature-trained T80 prediction on data evidence pipelines | Reproducibility package for a manuscript, with pipeline sensitivity analysis | Record documents a benchmark for how apparent predictability depends on evidence-processing choices | Not independently verified here as a peer-reviewed article. Relevant methodological context for avoiding unsupported generalization from one preprocessing workflow |

## Table 2. Cross-study synthesis

| Theme | What published evidence supports | What remains uncertain for our specific two accelerated-ageing archives | Planned or completed evidence test |
|---|---|---|---|
| Temperature-related degradation | Heat-stress studies and accelerated ageing records establish temperature as an important stressor | Are apparent rates robust to time window, startup transients and sample/pixel hierarchy? | Retention trajectories, matched-window kinetics, sample-aware uncertainty |
| Arrhenius kinetics | Arrhenius descriptions have been applied successfully in particular device/temperature/endpoint settings | Whether a common single activation energy applies to these specific architectures and measurement windows | `ln(k)` versus `1/T`; model residuals; bootstrap and sensitivity checks; label `E_a` as **apparent** |
| Multi-phase and recoverable behavior | Literature reports staged degradation, burn-in, light soaking and recovery | Which apparent T80 events represent sustained decline, interval-censoring or recoverable dips? | Gap-aware, sustained-threshold classification and baseline sensitivity |
| Degradation-model comparison | Statistical/physical and hybrid kinetic models have already been published | Whether flexibility in a stretched exponential survives independent-sample evaluation | Linear/exponential/stretched exponential comparisons with distinct temporal and grouped holdouts |
| Lifetime prediction | Dunlap-Shohl et al. demonstrate proof of concept for composition-specific held-out T80 forecasts | Whether the studied archives permit *reliable* out-of-sample T80 prediction rather than only good curve fits | Predicted-versus-observed T80 diagnostics; interval/right censoring; state failures and non-estimable predictions |
| Generalizability | Prior work demonstrates architecture heterogeneity, environmental effects and data-pipeline dependence | Whether trained results transfer across devices, studies, temperature bands and device architectures | Do not claim external transfer without genuinely comparable independent evidence |

## Dataset-to-research-question traceability

| Research question | Relevant experimental evidence | Supported inference boundary |
|---|---|---|
| How does temperature affect degradation? | Two accelerated ageing archives with nominal temperature groups | Describe measured MPPT PCE retention and compare robustly within known observation windows |
| Does a single Arrhenius law account for apparent rates? | Temperature-resolved archives | Apparent rate parameterization only; not a unique microscopic degradation mechanism |
| Which empirical degradation law has better held-out predictive performance? | Longitudinal PCE curves with sample/pixel grouping | Only the holdout groups and windows actually evaluated; avoid universal superiority claims |
| Can models predict device T80? | Curves reaching the retained-efficiency endpoint plus incomplete follow-up | Report observed, interval-censored and right-censored statuses separately; prediction error only when an evaluable future event exists |

## Scientific reporting rules

1. Keep the exact project title: **Thermal Degradation Kinetics and Lifetime Prediction of Perovskite Solar Cells**.
2. Report unsupported T80 reliability as a *negative/indeterminate result*, not a demonstrated lifetime forecasting capability.
3. Preserve distinction between training fit, temporal holdout, independent-sample test, and external generalization.
4. Device/pixel traces are not necessarily independent device replicates; account for sample/batch hierarchy.
5. Report time windows, temperature, stress and baseline definitions, threshold criteria, and data censoring.
6. All entries above distinguish original authors' findings from our appraisal; data-release pages are not substituted for peer-reviewed experimental interpretation.

## Primary sources and reproducibility

- Jacobsson et al. (2022): https://doi.org/10.1038/s41560-021-00941-3
- Hartono et al. (2023): https://doi.org/10.1038/s41467-023-40585-3
- Alsulami et al. (2024): https://doi.org/10.1039/D3TA05966A
- Dunlap-Shohl et al. (2024): https://doi.org/10.1039/D3TA06668A
- Flexible PSC module thermal stability (2024): https://doi.org/10.1016/j.solmat.2024.113148
- Dong et al. (2025): https://doi.org/10.1038/s41560-024-01689-2
- Accelerated ageing dataset (v2, 2026): https://doi.org/10.5281/zenodo.21242242
- Hartono MPPT ageing data (2023): https://doi.org/10.5281/zenodo.8185883
- Authors' PvkSOM code: https://github.com/noortitan/PvkSOM
