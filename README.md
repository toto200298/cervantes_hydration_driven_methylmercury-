# Hydration-Driven Inversion of the Methylmercury Halide Stability Series

**Alfonso Cervantes-Barragán**  
Dept. Mathematics, Physics and Data Sciences, Universidad del Norte  
Barranquilla, Colombia · barrangana@uninorte.edu.co / a.cervantes2012@hotmail.com

---

## Overview

This repository contains all computational data, optimized geometries,
thermochemical tables, and analysis scripts supporting the manuscript:

> **"Hydration-driven inversion of intrinsic affinity trends in methylmercury halides"**  
> *Submitted to Journal of Molecular Liquids*, 2026

The aqueous stability of methylmercury halide complexes follows
CH₃HgI > CH₃HgBr > CH₃HgCl > CH₃HgF — the **opposite** of what
gas-phase calculations predict. This work quantifies why.

---

## The Problem

| Complex | log K (exp.) | ΔG_aq (kcal/mol) | ΔG_gas (kcal/mol) |
|---------|-------------|------------------|-------------------|
| CH₃HgF  | 1.50 | −2.05  | −234.61 |
| CH₃HgCl | 5.25 | −7.16  | −199.59 |
| CH₃HgBr | 6.62 | −9.03  | −186.00 |
| CH₃HgI  | 8.60 | −11.73 | −172.71 |

Gas-phase affinities span **61.9 kcal/mol** but compress to only
**9.7 kcal/mol** in aqueous solution. The aqueous stability order
is completely reversed relative to the gas phase.

---

## Key Findings

**1. Near-complete thermodynamic compensation**  
The hydration-related contribution ΔΔG_solv opposes gas-phase
stabilization with a slope of −1.15 (R²_adj = 1.00) — 15% more
rapidly than the intrinsic affinity increases. This slight imbalance
is sufficient to reverse the entire stability sequence.

**2. Solvation attenuation by the CH₃Hg framework**  
Solvation free energies of neutral CH₃HgX complexes vary by only
~5.5 kcal/mol across the series, versus >54 kcal/mol for the free
halides. Electrostatic charge neutralization upon Hg–X bond formation
and the σ-donor effect of the methyl group are responsible.

**3. ΔG_solv(X⁻) as universal descriptor**  
The hydration free energy of the free halide controls both ΔΔG_solv
(R² = 0.96) and ΔG_aq (R² = 0.94), with a small slope (−0.168)
reflecting the near-cancellation of gas-phase and solvation contributions.

**4. Retention factor**  
Fluoride retains only **0.88%** of its gas-phase association energy
in solution; iodide retains **6.79%**.

---

## Methods

All calculations performed with **Gaussian 09** at three levels of theory:

| Method | Basis Set | Role |
|--------|-----------|------|
| APFD   | def2-SVP  | Primary reference |
| PBE0   | def2-SVP  | Consistency check |
| MP2    | def2-SVP  | Consistency check |

Scalar relativistic effects for Hg treated via def2 ECP (60 core electrons replaced).  
Thermodynamic cycle combines gas-phase free energies with experimental hydration
data from Marcus (1991) and formation constants from Schwarzenbach & Schellenberg (1965).

---

## Contact

Alfonso Cervantes-Barragán — Universidad del Norte, Barranquilla, Colombia  
barrangana@uninorte.edu.co / a.cervantes2012@hotmail.com
