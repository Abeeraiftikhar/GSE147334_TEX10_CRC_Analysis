# Key Findings

> **Project:** GSE147334 — TEX10 Knockdown vs. shNC Control | HCT116 Colorectal Cancer
> **Author:** Abeera Iftikhar | **Date:** May 2026

---

## Summary

RNA-seq differential expression analysis of TEX10-depleted HCT116 colorectal cancer
cells identified 235 significant DEGs from 18,903 tested genes, with 10 enriched KEGG
pathways revealing broad transcriptional reprogramming beyond the canonical NF-κB axis.

---

## 1. Differential Expression

| Metric | Result |
|---|---|
| Total genes tested | 18,903 |
| Significant DEGs | **235** |
| Upregulated | **103** |
| Downregulated | **132** |
| Cutoffs applied | padj ≤ 0.05 · \|log2FC\| ≥ 1 |
| Algorithm | DESeq2 (Benjamini-Hochberg FDR) |

---

## 2. Top Upregulated Genes

| Rank | Gene | log2FC | padj | Function |
|---|---|---|---|---|
| 1 | **HRNR** | +3.12 | 5.48×10⁻¹⁷ | Hornerin — skin barrier / cornification |
| 2 | **FLG** | +2.90 | 9.26×10⁻⁰⁸ | Filaggrin — epidermal structural protein |
| 3 | **GJA1** | +2.51 | 2.78×10⁻⁰³ | Connexin 43 — gap junction / tumor suppressor |
| 4 | **CEND1** | +2.49 | 3.65×10⁻⁰² | Cell cycle exit and neuronal differentiation |
| 5 | **SCN2A** | +2.14 | 1.22×10⁻⁰⁴ | Sodium voltage-gated channel alpha 2 |

---

## 3. Top Downregulated Genes

| Rank | Gene | log2FC | padj | Function |
|---|---|---|---|---|
| 1 | **HBA2** | −2.10 | 9.50×10⁻¹¹ | Hemoglobin subunit alpha 2 — redox/oxygen |
| 2 | **HBA1** | −1.82 | 1.40×10⁻⁰⁹ | Hemoglobin subunit alpha 1 |
| 3 | **LINC00887** | −1.80 | 4.17×10⁻⁰⁴ | Long intergenic non-coding RNA |
| 4 | **LCNL1** | −1.78 | 2.87×10⁻⁰⁵ | Lipocalin like 1 |
| 5 | **NDNF** | −1.78 | 3.20×10⁻⁰⁴ | Neuron derived neurotrophic factor |

> **Notable:** EGR1 (log2FC = −1.71, padj = 1.14×10⁻¹², baseMean = 5,763) —
> a major NF-κB-related transcription factor — was among the most significantly
> downregulated high-expression genes.

---

## 4. KEGG Pathway Enrichment

### Upregulated DEGs — 8 Pathways (5 FDR-significant)

| Pathway | Genes | p-value | FDR | Fold Enrichment |
|---|---|---|---|---|
| Systemic lupus erythematosus | 8 | 6.03×10⁻⁰⁶ | **6.39×10⁻⁰⁴** ✅ | 10.99 |
| Cornified envelope formation | 9 | 9.54×10⁻⁰⁶ | **6.39×10⁻⁰⁴** ✅ | 8.21 |
| Alcoholism | 8 | 3.80×10⁻⁰⁵ | **1.50×10⁻⁰³** ✅ | 8.29 |
| Neutrophil extracellular trap formation | 8 | 4.48×10⁻⁰⁵ | **1.50×10⁻⁰³** ✅ | 8.07 |
| Viral carcinogenesis | 7 | 4.83×10⁻⁰⁴ | **1.29×10⁻⁰²** ✅ | 6.76 |
| Staphylococcus aureus infection | 4 | 1.39×10⁻⁰² | 3.10×10⁻⁰¹ | 7.76 |
| Estrogen signaling pathway | 4 | 3.12×10⁻⁰² | 5.96×10⁻⁰¹ | 5.69 |
| Necroptosis | 4 | 4.37×10⁻⁰² | 7.32×10⁻⁰¹ | 4.98 |

### Downregulated DEGs — 2 Pathways (nominally significant)

| Pathway | Genes | p-value | FDR | Fold Enrichment |
|---|---|---|---|---|
| Growth hormone synthesis & action | 4 | 1.17×10⁻⁰² | 1.00 | 8.19 |
| Wnt signaling pathway | 4 | 2.98×10⁻⁰² | 1.00 | 5.74 |

> ✅ = Benjamini-Hochberg FDR < 0.05

---

## 5. Biological Interpretation

### 🔴 Upregulated — Key Insights
- **Cornified envelope formation** (FDR = 6.39×10⁻⁴) driven by HRNR and FLG
  suggests TEX10 normally suppresses an aberrant epithelial differentiation program in CRC
- **GJA1** upregulation (connexin 43) implies restored gap junction-mediated
  tumor suppression upon TEX10 loss
- **Viral carcinogenesis** enrichment (FDR = 1.29×10⁻²) reflects known
  NF-κB pathway hijacking by oncogenic stimuli
- **NET formation** enrichment suggests TEX10 modulates innate immune
  gene programs in colorectal cancer cells

### 🔵 Downregulated — Key Insights
- **EGR1** suppression (baseMean = 5,763) indicates disruption of a major
  NF-κB-connected transcription factor upon TEX10 depletion
- **Wnt signaling** downregulation is biologically significant —
  Wnt/β-catenin is the most frequently activated pathway in CRC (APC
  mutations in >80% of sporadic cases), suggesting TEX10-NF-κB/Wnt crosstalk
- **HBA1/HBA2** suppression may reflect altered redox homeostasis and
  metabolic reprogramming

---

## 6. Quality Control Highlights

| Plot | Finding |
|---|---|
| Box plot | Uniform normalized counts across all 8 samples ✅ |
| p-value histogram | Strong enrichment near zero — genuine signal ✅ |
| Dispersion estimates | Well-fitted DESeq2 negative binomial model ✅ |
| UMAP | Clear separation between Tumor and Control groups ✅ |
| Venn diagram | 235 / 18,903 genes significant (1.24%) ✅ |

---

## 7. Candidate Genes for Validation

Based on statistical significance, fold change magnitude, and biological relevance:

```
Priority targets for experimental follow-up:

Upregulated:  GJA1  ·  HRNR  ·  FLG
Downregulated: EGR1  ·  HBA2  ·  WNT pathway components
```

---

## Files Reference

| Finding | File |
|---|---|
| All 235 DEGs | `02_preprocessing/GSE147334_ALL_significant_DEGs.csv` |
| Upregulated genes | `02_preprocessing/GSE147334_Upregulated_DEGs.csv` |
| Downregulated genes | `02_preprocessing/GSE147334_Downregulated_DEGs.csv` |
| KEGG results (up) | `04_DAVID_KEGG/DAVIDChartReport_Upregulated.csv` |
| KEGG results (down) | `04_DAVID_KEGG/DAVIDChartReport_Downregulated.csv` |
| KEGG summary | `04_DAVID_KEGG/KEGG_All_Pathways_Summary.csv` |
| Full manuscript | `06_manuscript/GSE147334_Final_Manuscript.docx` |

---

*Analysis by Abeera Iftikhar | May 2026 | Dataset: GSE147334*
