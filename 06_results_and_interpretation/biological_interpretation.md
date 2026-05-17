# Biological Interpretation

> **Project:** GSE147334 — TEX10 Knockdown vs. shNC | HCT116 Colorectal Cancer
> **Author:** Abeera Iftikhar | **Date:** May 2026

---

## Overview

TEX10 (Testis-Expressed Gene 10) promotes colorectal cancer (CRC) cell proliferation
by enhancing NF-κB transcriptional activity. Its knockdown in HCT116 CRC cells
produced 235 significant DEGs and 10 enriched KEGG pathways, revealing that TEX10
regulates transcriptional programs far beyond the canonical NF-κB axis — including
epithelial differentiation, immune signaling, gap junction communication, lipid
metabolism, and Wnt pathway activity.

---

## 1. TEX10 and NF-κB Signaling

TEX10 was identified through RNAi screening as a positive regulator of NF-κB
activity in HCT116 CRC cells. NF-κB drives expression of genes promoting tumor
cell survival, proliferation, invasion, and immune evasion. Upon TEX10 knockdown:

- NF-κB transcriptional output is reduced
- Downstream target genes are suppressed
- Cell proliferation is inhibited

The significant downregulation of **EGR1** (Early Growth Response 1;
log2FC = −1.71, padj = 1.14×10⁻¹², baseMean = 5,763) — a zinc finger transcription
factor that operates within the NF-κB regulatory network — suggests TEX10 maintains
EGR1 expression as part of its pro-tumorigenic transcriptional program. EGR1 has
established roles in cell growth, differentiation, and apoptosis modulation in CRC,
and its suppression upon TEX10 loss indicates disruption of a broader
NF-κB-connected gene regulatory axis.

---

## 2. Cornified Envelope Formation — Aberrant Differentiation Program

**Top enriched pathway:** Cornified envelope formation (9 genes, FDR = 6.39×10⁻⁴)

The two most highly upregulated genes — **HRNR** (hornerin; log2FC = +3.12) and
**FLG** (filaggrin; log2FC = +2.90) — are both core components of the epidermal
cornification machinery, normally expressed in terminally differentiating
keratinocytes of the skin.

Their significant upregulation in HCT116 CRC cells upon TEX10 knockdown suggests:

- TEX10 actively **suppresses an aberrant cornification gene program** in colorectal
  cancer cells
- Loss of TEX10 **releases this suppression**, allowing ectopic expression of
  skin barrier genes
- This may reflect **altered cell identity** — a shift away from the proliferative
  CRC phenotype toward a more differentiated state
- Aberrant cornification gene expression has been reported in other epithelial
  cancers as a marker of differentiation and reduced malignancy

> **Implication:** TEX10 may function as a suppressor of terminal differentiation
> in CRC, maintaining cells in a proliferative, dedifferentiated state via NF-κB.

---

## 3. GJA1 (Connexin 43) — Gap Junction Tumor Suppression

**HRNR** | log2FC = +2.51 | padj = 2.78×10⁻³

GJA1 encodes Connexin 43, the most abundantly expressed gap junction protein in
the colon. Gap junctions are intercellular channels that enable direct cell-to-cell
communication of small molecules, ions, and signaling mediators.

In colorectal cancer:
- GJA1 expression is frequently **silenced or reduced** compared to normal colon
- Its loss promotes tumor cell **proliferation, invasion, and metastasis**
- Restoration of GJA1 in CRC cells **suppresses tumor growth** in vitro and in vivo

The upregulation of GJA1 upon TEX10 knockdown strongly suggests:

- TEX10 normally **suppresses GJA1 expression** in CRC cells, likely through
  NF-κB-mediated transcriptional repression
- TEX10 depletion **restores gap junction communication**, reducing proliferative
  capacity
- This is consistent with the observed reduction in HCT116 cell growth upon
  TEX10 knockdown

> **Implication:** TEX10-NF-κB may silence GJA1 as a mechanism of maintaining
> CRC cell proliferation and intercellular isolation — a targetable vulnerability.

---

## 4. Hemoglobin Subunits — Metabolic Reprogramming

**HBA2** | log2FC = −2.10 | padj = 9.50×10⁻¹¹
**HBA1** | log2FC = −1.82 | padj = 1.40×10⁻⁰⁹

While classically associated with erythroid lineages, hemoglobin alpha subunit
expression has been documented in non-erythroid cells including colorectal
epithelial cells and CRC lines.

In cancer cells, HBA1/HBA2 are linked to:
- **Intracellular oxygen sensing** and reactive oxygen species (ROS) buffering
- **Redox homeostasis** — protection against oxidative stress
- **Metabolic state regulation** under hypoxic tumor microenvironments

Their significant downregulation upon TEX10 loss suggests:
- TEX10 may support **HBA-mediated redox protection** in CRC cells
- Loss of TEX10 disrupts this protection, potentially increasing oxidative
  stress sensitivity
- This may contribute to the observed reduction in CRC cell viability

---

## 5. Viral Carcinogenesis — NF-κB Pathway Hijacking

**Pathway:** Viral carcinogenesis (7 genes, FDR = 1.29×10⁻²)

The enrichment of the Viral carcinogenesis KEGG pathway among upregulated DEGs
is mechanistically consistent with TEX10-NF-κB biology. Oncogenic viruses
(HPV, EBV, HBV, HTLV-1) transform host cells by constitutively activating
NF-κB — the same pathway enhanced by TEX10 in CRC.

Genes enriched in this pathway overlap with NF-κB target genes and
chromatin-regulatory factors. Their upregulation upon TEX10 knockdown may reflect
a **compensatory transcriptional response** to NF-κB suppression, or direct
de-repression of viral carcinogenesis pathway components normally silenced by
TEX10-driven NF-κB activity.

> **Implication:** The viral carcinogenesis pathway shares molecular machinery
> with TEX10-NF-κB signaling, reinforcing the oncogenic relevance of TEX10 in CRC.

---

## 6. Neutrophil Extracellular Trap Formation — Immune Regulation

**Pathway:** NET formation (8 genes, FDR = 1.50×10⁻³)

Neutrophil extracellular traps (NETs) are web-like structures of DNA, histones,
and antimicrobial proteins released by neutrophils during innate immune responses.
In cancer:

- NETs have been shown to **promote tumor metastasis** by trapping circulating
  tumor cells and remodeling the extracellular matrix
- NET-related gene expression in tumor cells may reflect **immune mimicry** —
  cancer cells co-opting innate immune pathways
- NF-κB is a master regulator of NET formation genes

Upregulation of NET formation genes upon TEX10 knockdown suggests:
- TEX10 normally **suppresses innate immune gene expression** in CRC cells
- Its depletion allows expression of NET-related genes, potentially altering
  tumor-immune interactions
- This pathway represents an emerging therapeutic axis in CRC immunotherapy

---

## 7. Wnt Signaling — CRC's Most Mutated Pathway

**Pathway:** Wnt signaling (4 genes, p = 0.0298, nominally significant)

The Wnt/β-catenin signaling pathway is the **most frequently activated oncogenic
pathway in colorectal cancer**, with APC tumor suppressor mutations present in
over 80% of sporadic CRC cases. Wnt activation drives CRC initiation,
stem cell maintenance, and tumor progression.

The downregulation of 4 Wnt signaling components upon TEX10 knockdown is
biologically significant:

- Suggests a **TEX10-NF-κB/Wnt signaling crosstalk** in CRC cells
- TEX10 may sustain Wnt pathway activity indirectly through NF-κB-mediated
  gene regulation
- Loss of TEX10 partially suppresses Wnt signaling, contributing to reduced
  proliferative capacity

> **Important note:** This pathway did not achieve Benjamini FDR significance
> (FDR = 1.00), indicating the result is nominally significant only and
> requires experimental validation.

---

## 8. Growth Hormone Signaling

**Pathway:** Growth hormone synthesis, secretion and action (4 genes, p = 0.0117)

Growth hormone (GH) signaling through GH receptor activates JAK2-STAT5, MAPK,
and PI3K-AKT cascades — all of which intersect with NF-κB signaling. The
downregulation of GH pathway genes in TEX10-depleted cells suggests:

- TEX10-NF-κB may sustain **GH-downstream signaling** in CRC
- Loss of TEX10 reduces this activity, contributing to anti-proliferative effects
- GH pathway-NF-κB crosstalk in CRC is an understudied area with potential
  therapeutic relevance

---

## 9. Integrated Model

```
          TEX10 (active in CRC)
               │
               ▼
         NF-κB activation
               │
    ┌──────────┼──────────────────┐
    ▼          ▼                 ▼
Suppresses  Maintains         Sustains
  GJA1     EGR1 expression   Wnt / GH
(gap jxn)  (transcription    signaling
            factor network)
    │
    ▼
Promotes CRC proliferation
Blocks differentiation
Evades immune surveillance


      TEX10 knockdown
               │
               ▼
         NF-κB suppressed
               │
    ┌──────────┼──────────────────┐
    ▼          ▼                 ▼
GJA1 ↑      EGR1 ↓            Wnt ↓
Cornification  Immune genes ↑   HBA1/2 ↓
genes ↑     (NET, viral        (redox)
(HRNR, FLG)  carcinogenesis)
    │
    ▼
Reduced proliferation
Partial re-differentiation
Altered immune gene profile
```

---

## 10. Candidate Targets for Experimental Validation

| Gene / Pathway | Direction | Priority | Rationale |
|---|---|---|---|
| **GJA1** | ↑ | 🔴 High | Known CRC tumor suppressor; TEX10-NF-κB may silence it |
| **EGR1** | ↓ | 🔴 High | Major NF-κB-connected TF; high baseMean; strong padj |
| **HRNR / FLG** | ↑ | 🟡 Medium | Cornification axis; novel in CRC context |
| **Wnt signaling** | ↓ | 🟡 Medium | Most mutated CRC pathway; TEX10 crosstalk unexplored |
| **HBA1 / HBA2** | ↓ | 🟡 Medium | Redox/metabolic axis; novel TEX10 connection |
| **NET formation** | ↑ | 🟢 Exploratory | Immune gene mimicry; emerging CRC immunology area |

---

## 11. Study Limitations

- Analysis is based on **HCT116 cell line** data only — may not fully reflect
  primary tumor biology or patient heterogeneity
- This is a **knockdown experiment**, not tumor-vs-normal tissue; DEGs reflect
  TEX10-dependent regulation rather than classical cancer transcriptomics
- The downregulated KEGG pathways (Wnt, GH) did **not achieve FDR significance**
  — treat as hypothesis-generating only
- Small sample size (n=3 knockdown vs. n=5 control) limits statistical power
  for lower-fold-change genes
- Protein-level validation (Western blot, IHC) is needed to confirm
  transcriptomic findings

---

## References

1. Wang X, et al. (2021). RNAi Screening Identifies that TEX10 Promotes CRC Proliferation via NF-κB. *GEO: GSE147334.*
2. Love MI, et al. (2014). DESeq2. *Genome Biology*, 15, 550.
3. Huang DW, et al. (2009). DAVID bioinformatics. *Nature Protocols*, 4, 44–57.
4. Kanehisa M, Goto S. (2000). KEGG. *Nucleic Acids Research*, 28, 27–30.
5. Sung H, et al. (2021). Global Cancer Statistics 2020. *CA Cancer J Clin*, 71, 209–249.

---

*Analysis by Abeera Iftikhar | May 2026 | Dataset: GSE147334*
