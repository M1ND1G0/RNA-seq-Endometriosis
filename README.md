# Differential Gene Expression Between Ectopic and Eutopic Endometrium Highlights Cancer-Linked Pathways in Endometriomas

This repository contains an independent RNA-seq analysis comparing ectopic ovarian endometrioma tissue to paired eutopic endometrial samples, aiming to identify molecular signatures associated with early oncogenic risk.

## 📄 Files Included

- `Final_Report_ENDO.pdf` – Full unpublished manuscript with all figures, tables, methods, and results  
- `RMarkdown_analysis_ENDO.pdf` – RMarkdown-based analysis pipeline with code

## 🔍 Project Overview

- **Dataset**: 10 ectopic (ENDO) vs. 10 eutopic (CTL) samples  
- **Source**: [GEO GSE279835](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE279835)  
- **Pipeline**:
  - Preprocessing: FastQC, Trimmomatic, HISAT2, HTSeq (via Galaxy)
  - Analysis: DESeq2, DAVID, GSEA (MSigDB Hallmark sets)
  - Visualization: EnhancedVolcano, ggplot2, pheatmap

## 🧬 Key Findings

- 7,248 differentially expressed genes (FDR < 0.05)
- Downregulation of *TP53*, *BRCA1*, *CCNE2*; upregulation of *ATM*
- Enriched pathways in DNA repair, cell cycle checkpoints, and immune regulation
- Novel DEGs identified: *C9orf152*, *RP11-6E9.4*

## 📂 Contents

All tables and figures are included in `Final_Report_ENDO.pdf`.  
`RMarkdown_analysis_ENDO.pdf` contains the full reproducible analysis code and visual outputs.

## 🧪 How to Reproduce

This project used Galaxy for initial RNA-seq processing and R/Bioconductor for differential expression and enrichment analysis. See the RMarkdown PDF for code and packages used.

## 🙏 Acknowledgments

- Data: Frisendahl et al., GSE279835  
- Tools: Galaxy, Bioconductor (DESeq2, EnhancedVolcano), DAVID, GSEA

---

*This project was conducted independently and is not affiliated with any institution.*
