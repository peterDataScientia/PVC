# Thermal Degradation Kinetics and Lifetime Prediction of Perovskite Solar Cells

## Research project

This repository documents an MSc Physics research study of temperature-dependent photovoltaic degradation kinetics and evaluation of T80 lifetime prediction in perovskite solar cells.

**Research title (retained without modification):**  
**Thermal Degradation Kinetics and Lifetime Prediction of Perovskite Solar Cells**

## Research questions

1. How does temperature influence the measured degradation trajectories and apparent kinetic rates of perovskite solar cells?
2. To what extent do Arrhenius-type kinetics describe the temperature dependence of experimentally estimated degradation rates?
3. How do linear, exponential and stretched-exponential descriptions compare under held-out-data evaluation?
4. How reliably can degradation models predict T80 from observed ageing measurements?

## Data sources and scope

- Experimental accelerated-ageing datasets (2024, 2026): https://doi.org/10.5281/zenodo.10902908 and https://doi.org/10.5281/zenodo.21242242
- Complementary ageing-curve dataset (2023; 2,245 MPPT curves): https://doi.org/10.5281/zenodo.8185883 ; original analysis source: https://github.com/noortitan/PvkSOM
- The two accelerated-ageing archives analysed in the project have been reported as 146 and 144 device/pixel traces, respectively, across nominal 25–65 °C conditions. Their time windows and experimental systems are not automatically exchangeable.

The third dataset's published 150-hour curves do not provide per-curve temperature and device metadata in the released pickle, and therefore should not be treated as directly temperature-resolved without a verified metadata mapping.

## Evidence and interpretation

Temperature-related PCE retention differences and apparent degradation kinetics can be studied from the temperature-resolved datasets. Previously evaluated models did **not** establish robust, generalizable T80 prediction. Observed threshold events must be distinguished from model-extrapolated lifetimes; temporal-holdout accuracy is not independent sample-group validation. Do not infer unique microscopic degradation mechanisms solely from apparent activation energies.

## Literature review

See [Literature synthesis matrix](literature/LITERATURE_SYNTHESIS_MATRIX.md) for source-checked studies, reported methods, findings, critical appraisal, research-gap synthesis and dataset relevance.

## Attribution

Original experimental data belong to their respective authors. Follow source licenses and cite original articles and dataset DOIs. This repository does not present its secondary analyses as newly generated laboratory experiments.
