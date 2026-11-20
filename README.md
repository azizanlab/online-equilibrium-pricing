# Online Learning for Equilibrium Pricing in Markets under Incomplete Information

**Authors:** Devansh Jalota\*, Haoyuan Sun\*, Navid Azizan

\* Equal contribution

**Paper:** [arXiv:2303.11522](https://arxiv.org/abs/2303.11522)

This repository contains the code for the numerical experiments in the paper (Section 7 and Appendix EC.3).

## Source Files

- `FixedDemand.ipynb`: validates Theorem 1 (Algorithm 1, fixed costs and fixed demand); its output corresponds to Figures 1 and EC.1–EC.4.
- `VaryingDemand_CAISO_2025.ipynb`: validates Theorem 2 (Algorithm 3, fixed costs and time-varying demand); its output corresponds to Figures 2 and EC.5–EC.7.
- `TimeVaryingCosts.ipynb`: validates Theorem 3 (Algorithm 4, time-varying costs with contexts); its output corresponds to Figures 3 and EC.8.
- `GD_EnergyMarkets.ipynb`: validates Proposition 3 using online dual sub-gradient descent (Algorithm 5); its output corresponds to Figure EC.9.

In `FixedDemand.ipynb` and `VaryingDemand_CAISO_2025.ipynb`, set the `cost_type` variable to select the different market instances discussed in Section 7.1:

- `'piecewise'`: Instance 1, a single supplier with a piecewise quadratic cost.
- `'three'`: Instance 2, three suppliers with quadratic costs.
- `'log'`: Instance 3, a single supplier with a log-barrier cost.

## Data

The demand data in `caiso_hourly_load_2025_combined.csv` comes from the California Independent System Operator (CAISO), [Historical EMS hourly load](https://www.caiso.com/library/historical-ems-hourly-load).

## Citation

```bibtex
@article{jalota2026online,
  title   = {Online Learning for Equilibrium Pricing in Markets under Incomplete Information},
  author  = {Jalota, Devansh and Sun, Haoyuan and Azizan, Navid},
  journal = {Operations Research},
  year    = {2026},
  note = {Forthcoming}
}
```
