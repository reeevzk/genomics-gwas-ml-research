
# Genotype–Phenotype Association Modeling for Drought Tolerance

This repository documents a machine learning–driven genomics research project focused on identifying
genotype–phenotype associations related to drought tolerance in *Oryza sativa* (rice).

The work applies GWAS-style statistical models and population-structure correction techniques to analyze
high-dimensional genomic data. Further, the project employs Quantitative Trait Loci (QTL) analysis for identification of genotype-phenotype relations. Due to data-use and confidentiality constraints, source code and raw datasets
are not publicly released. This repository serves as a technical summary and research artifact.

## Problem

Environmental stressors such as drought significantly impact crop yield. This project investigates whether
specific genetic variants (SNPs) are statistically associated with phenotypes known to correlate with drought
tolerance.

From an ML perspective, the problem is characterized by:
- High-dimensional feature space (~44,000 SNPs)
- Limited sample size (413 rice varieties)
- Strong population structure requiring explicit correction

## Modeling Approach

The analysis employs Genome-Wide Association Study (GWAS) methodologies with a focus on statistical rigor
and confounder control.

Key techniques include:
- Linear mixed models to account for population stratification
- Kinship matrix estimation from genotypic data
- LOD score (-log10 P-value)–based feature significance ranking
- Threshold-based selection of statistically significant loci

Phenotypes analyzed include:
- Plant height
- Seed length-to-width ratio
- Amylose content
- Protein content


## Results

The analysis identified multiple SNPs with high statistical significance associated with drought-related
phenotypes. Several of these loci were linked to genes involved in:
- Stress and osmotic response
- Protein folding and degradation
- Seed development and early growth stages

Orthologous gene analysis in *Arabidopsis thaliana* and *Zea mays* further supported the biological relevance of the identified loci.

Figures and plots included in this repository visualize key GWAS results.

---

## Recognition

This research was conducted as part of independent computational genomics work and was supported by:
- **AAAS Fellowship**
- **Syngenta Community Grant**

---

## Confidentiality Notice

Source code, datasets, and intermediate artifacts are not publicly available due to data-use agreements and
confidentiality constraints. The methodology and results presented here reflect the technical scope of the work
without exposing proprietary materials.

---

## Citation

If referencing this work, please cite the included paper.
