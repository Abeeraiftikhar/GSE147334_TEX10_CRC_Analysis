# 🧬  GSE147334_TEX10_CRC_Analysis

A complete transcriptomic and pathway enrichment analysis pipeline for investigating the role of TEX10 in colorectal cancer (CRC) using the public GEO dataset GSE147334.
This project integrates differential gene expression (DEG) analysis, GEO2R quality control visualization, and KEGG pathway enrichment analysis to identify molecular alterations associated with TEX10 knockdown in CRC.

## 📌 Project Overview

This repository presents an end-to-end bioinformatics workflow built from publicly available GEO expression data. The analysis focuses on identifying significantly altered genes and enriched biological pathways after TEX10 knockdown in colorectal cancer samples.

## The pipeline includes:

-GEO dataset preprocessing

-DEG filtering and classification

-GEO2R quality-control visualizations

-KEGG pathway enrichment analysis using DAVID

-Publication-ready plots and manuscript files

## ⚙️ Workflow Pipeline

### 1️⃣ Raw Data Collection
-Downloaded GEO series matrix and GEO2R output tables from NCBI GEO.

-Organized metadata and experimental conditions.

### 2️⃣ DEG Filtering & Processing

-Applied filtering criteria:

-Adjusted p-value (padj) < 0.05

-|log2FC| > 1

## Generated:

-Significant DEG tables

-Upregulated gene list

-Downregulated gene list

-Excel export with formatted sheets

### 3️⃣ GEO2R Quality Control Visualizations

Generated multiple QC and exploratory plots:

-Volcano Plot

-MA Plot

-UMAP Plot

-Venn Diagram

-Box Plot

-P-value Distribution

-Mean-Variance Trend Plot

These visualizations help validate normalization quality and DEG distribution.

### 4️⃣ KEGG Pathway Enrichment Analysis

Performed KEGG enrichment using DAVID Functional Annotation Tool.

Inputs

-Upregulated gene symbols

-Downregulated gene symbols

-Outputs

-Enriched pathway reports

-Combined KEGG pathway summary

-Visualization-ready enrichment tables

### 5️⃣ KEGG Visualization

Generated publication-style pathway figures including:

-Horizontal KEGG Bar Chart

-KEGG Bubble Plot

-Combined Multi-panel Figure

## 📊 Key Findings

-Identified 235 significant DEGs associated with TEX10 knockdown.

-Detected multiple enriched pathways linked to:

-Cell proliferation

-Cancer progression

-Signal transduction

-Cellular metabolic regulation

The results provide insights into the molecular role of TEX10 in colorectal cancer progression.

## 🛠️ Tools & Technologies

-Bioinformatics Platforms

-GEO2R

-DAVID

-NCBI GEO

-Programming & Visualization

-Python

-Pandas

-NumPy

-Matplotlib

-Seaborn

-Development Environment

-Google Colab
-Jupyter Notebook
