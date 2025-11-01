# Synthetic Stress–Strain Curves for Fe–C Steels — Commercial Sample  
**Synarch Labs — Synthetic Data Intelligence**

---

## Executive Summary

This document presents a **commercial-grade sample of nine synthetic stress–strain curves** representing **iron–carbon (Fe–C) steels** under different thermomechanical conditions.  
The dataset provides a **realistic, physics-consistent reference** for evaluating analytical models, validating computational workflows, and exploring the integration of synthetic data in materials research.

Each curve reproduces the **characteristic behavior** of carbon steels across the **elastic, plastic, and fracture regimes**, including the expected contrasts between **annealed**, **normalized**, and **quenched–tempered** states.  
Mechanical responses were parameterized and calibrated according to verified literature ranges, ensuring that the profiles are both **statistically coherent** and **physically credible**.

This release demonstrates how **synthetic materials data** can support **advanced engineering and data-science applications**. Users can expect a controlled yet realistic dataset that behaves consistently with experimental observations, enabling **benchmark testing**, **model validation**, and **machine learning calibration**.  

Each dataset instance maintains internal consistency through **multi-stage quality verification**. Key parameters such as elastic slope, yield ratio, and monotonic strain progression are automatically validated. Minor stochastic variability is introduced to emulate laboratory dispersion, offering a **balance between realism and reproducibility**.

The purpose of this sample is not to represent an exhaustive database, but to illustrate the **level of control, coherence, and realism** achievable through physics-guided synthetic data generation.  
Full-scale datasets can extend these concepts across **broader composition ranges**, **additional alloy systems**, or **varying temperature conditions**, accelerating predictive modeling and digital materials design.

---

## Why This Dataset Matters

- ️ **Physics-informed accuracy:** Realistic mechanical behavior of Fe–C steels, aligned with verified engineering data.  
-  **Microstructural diversity:** Includes annealed, normalized, and quenched–tempered conditions.  
- **High-fidelity resolution:** Dense sampling across full deformation paths, from elasticity to fracture.  
-  **Laboratory-grade realism:** Controlled variability emulates real experimental dispersion.  
- **Validated consistency:** Built-in QC flags ensure physical plausibility and numerical continuity.

---

## Contents

| File | Description |
|------|--------------|
| **stress_strain_series.csv** | Contains 9×100 rows of strain–stress pairs with identifiers and outlier flags. |
| **stress_strain_metadata.csv** | Provides per-curve parameters such as carbon content, Young’s modulus, σᵧ, UTS, fracture strain, work-hardening constants, and QC results. |

---

## Key Variables (Metadata)

| Variable | Unit | Purpose |
|-----------|------|----------|
| `carbon_pct` | % | Weight fraction of carbon, typically 0.25–0.5 % for hypoeutectoid steels. |
| `elastic_modulus_GPa` | GPa | Young’s modulus (~200 GPa for Fe–C steels). |
| `yield_strength_MPa` | MPa | σᵧ — onset of plastic flow. |
| `ultimate_strength_MPa` | MPa | Maximum stress before necking. |
| `fracture_strain` | – | Strain at fracture (ductility measure). |
| `hardening_coefficient_K` | MPa | Hollomon coefficient K in σ = K·εⁿ. |
| `hardening_exponent_n` | – | Work-hardening exponent n (≈ 0.10–0.25). |
| `hall_petch_ky` | MPa·mm⁻½ | Hall–Petch constant linking grain size and yield strength. |
| `necking_parameter_k` | – | Controls post-UTS softening. |
| `grain_size_um` | μm | Average grain size used in Hall–Petch relation. |
| `qc_*` | – | Boolean QC flags for elastic slope, UTS/σᵧ ratio, and curve monotonicity. |

---

## Intended Use

This dataset is provided for **evaluation, demonstration, and exploratory analysis**.  
It helps researchers, engineers, and developers understand the structure, consistency, and realism achievable through **physics-aligned synthetic data**.

### Typical applications
- **Education:** Demonstrating elastic-plastic deformation, strain hardening, and process–property relationships.  
- **Machine learning prototyping:** Benchmarking algorithms that predict or reconstruct stress–strain curves.  
- **Software & model validation:** Testing FEM solvers, constitutive models, and data pipelines using controlled reference curves.

> ⚠️ This sample is **not intended for commercial deployment or large-scale model training**.  
> It serves as a **compact, high-quality reference** for evaluating reproducibility, realism, and dataset structure.

---

## Licensing & Availability

This sample is released under a **Non-Commercial Evaluation Licence (CC BY-NC 4.0)**.  
Redistribution or inclusion in commercial products is **not permitted**.

To request **academic collaboration**, **commercial licensing**, or **custom dataset generation** (including other alloys or process parameters), please contact the Synarch Labs team.

---

## Contact & Support

**Synarch Labs — Synthetic Data Intelligence**  
📧 Email: [synarchlabs@gmail.com](mailto:synarchlabs@gmail.com) | [synarchlabs@proton.me](mailto:synarchlabs@proton.me)
We are committed to supporting researchers, engineers, and developers in harnessing **high-quality synthetic data**.

---

