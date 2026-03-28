# LSDV132-BCL2-Characterization

In silico characterization of the LSDV132 protein of Lumpy Skin Disease Virus (LSDV) — revealing its BCL-2-like nature and identifying pelcitoclax as a top inhibitor candidate.

> **Published in:** Heliyon, Vol. 10, March 2024
> **DOI:** [10.1016/j.heliyon.2024.e27657](https://doi.org/10.1016/j.heliyon.2024.e27657)
> **Access:** Open Access (Creative Commons)

---

## Overview

Lumpy Skin Disease Virus (LSDV) belongs to the Poxviridae family and causes serious economic losses in livestock. The LSDV132 protein is one of its structural proteins whose function was previously unknown — no relevant study had been reported about it prior to this work.

This study is the **first in-silico characterization of LSDV132**, revealing that it possesses BCL-2-like motifs, suggesting a role in modulating host cell apoptosis — a key mechanism viruses use to evade immune responses.

**Top finding:** Pelcitoclax showed the highest docking score (-9.1841 kcal/mol) among all screened BCL-2 inhibitors, identifying it as a potential therapeutic inhibitor of LSDV132.

---

## Pipeline

```
LSDV132 Protein Sequence
        ↓
Physiochemical Characterization (ProtParam)
        ↓
Phosphorylation Site Prediction
        ↓
Secondary Structure Prediction
        ↓
3D Structure Modeling & Refinement (DeepRefiner)
        ↓
Model Validation (Ramachandran Plot)
        ↓
Pocket/Active Site Identification
        ↓
KEGG & Protein Family Classification → BCL-2-like motifs confirmed
        ↓
BCL-2 Inhibitor Screening (ChEMBL database)
        ↓
Molecular Docking
        ↓
Best Inhibitor → Pelcitoclax (-9.1841 kcal/mol)
```

---

## Key Findings

### Physiochemical Properties
- Instability index: **30.89%** → protein is stable
- Multiple phosphorylation sites identified → involvement in apoptosis regulation and cell signaling

### Structural Analysis
- Secondary and 3D structure predicted and refined using DeepRefiner
- Ramachandran plot validation: **93.6% residues in favored region** → high quality model
- Multiple binding pockets identified and ranked by size and volume

### BCL-2-like Nature
- KEGG analysis and protein family classification confirmed **Poxvirus-BCL-2-like motifs**
- LSDV132 likely modulates **host cell apoptosis** — a viral immune evasion strategy

### Molecular Docking Results

| Compound | Category | Docking Score |
|----------|----------|--------------|
| **Pelcitoclax** | **BCL-2 inhibitor** | **-9.1841 kcal/mol ✓ Best** |
| Other ChEMBL compounds | BCL-2 inhibitors | < -9.18 kcal/mol |

> Pelcitoclax is identified as a potential inhibitor of LSDV132 protein.

---

## Repository Structure

```
LSDV132-BCL2-Characterization/
├── figures/
│   ├── secondary_structure_LSDV132.png
│   ├── 3D_model_LSDV132.png
│   ├── ramachandran_plot.png
│   ├── binding_pockets.png
│   └── docking_pelcitoclax.png
├── results/
│   └── docking_scores_summary.csv
└── README.md
```

---

## Tools & Databases Used

| Tool / Database | Purpose |
|----------------|---------|
| `ProtParam` (ExPASy) | Physiochemical characterization |
| `NetPhos` | Phosphorylation site prediction |
| `PSIPRED` | Secondary structure prediction |
| `DeepRefiner` | 3D model refinement |
| `PROCHECK` | Ramachandran plot validation |
| `fpocket` | Active site/pocket prediction |
| `KEGG` | Pathway & protein family classification |
| `ChEMBL` | BCL-2 inhibitor library |
| `MOE` | Molecular docking |
| `PyMOL` | 3D structure visualization |

---

## Citation

If you use this work, please cite:

> Sarwar, M.F.\*, Waseem, Q.U.\*, Awan, M.F., Ali, S., Ahmad, A., Malook, S.U., & Ali, Q. (2024). In-silico characterization of LSDV132 protein divulged its BCL-2-like nature. *Heliyon*, 10(6), e27657. https://doi.org/10.1016/j.heliyon.2024.e27657

*\* Co-first authors with equal contribution*

---

## Authors

**Muhammad Farhan Sarwar & Qurat ul Ain Waseem** (Co-first authors)
Department of Biotechnology, Knowledge Unit of Science
University of Management and Technology (UMT), Sialkot, Pakistan

- LinkedIn: [quratulain-waseem-239310353](https://www.linkedin.com/in/quratulain-waseem-239310353)
- ORCID: [0009-0003-9735-5632](https://orcid.org/0009-0003-9735-5632)

---

> This is the first computational characterization of LSDV132 protein. The findings suggest LSDV132 as a potential drug target for Lumpy Skin Disease Virus therapy.
