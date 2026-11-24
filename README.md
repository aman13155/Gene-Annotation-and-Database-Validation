# 🧬 Gene Annotation and Database Validation

### Gene Identification, Annotation and Cross-Database Validation Using NCBI, MyGene.info and UniProt

## 📌 Overview

This project focuses on gene identification, annotation, and biological database availability analysis using the Adamson single-cell RNA-seq (Perturb-seq) dataset.

It integrates bioinformatics tools and biological database APIs to identify gene symbols, retrieve gene metadata, map gene identifiers, and evaluate gene availability across multiple biological databases.

The framework also explores computational gene candidate discovery and biological validation using external resources.

## 🎯 Objectives

- Extract gene symbols and metadata from single-cell datasets.
- Retrieve gene annotations using MyGene.info.
- Identify gene records through NCBI Entrez.
- Compare gene availability across NCBI and UniProt.
- Identify genes missing from selected biological databases.
- Perform gene identifier mapping and annotation analysis.
- Explore computationally identified gene candidates.

## 🔬 Research Workflow

```text
Adamson Perturb-seq Dataset
          |
          v
  Gene Extraction
          |
          v
   Gene Symbol Mapping
          |
     +----+-----+
     |          |
     v          v
 MyGene.info   NCBI Entrez
     |          |
     v          v
 Gene Metadata Gene Records
     |          |
     +----+-----+
          |
          v
   UniProt Database
          |
          v
 Cross-Database Comparison
          |
          v
 Gene Availability Analysis
          |
          v
 CSV Results and Validation
```

## 🧪 Technologies and Tools

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Scanpy | Single-cell data analysis |
| AnnData | Gene expression data management |
| Pandas & NumPy | Data processing |
| MyGene.info | Gene annotation and identifier mapping |
| NCBI Entrez | NCBI Gene database queries |
| UniProt REST API | Protein and gene-related information |
| Biopython | Biological database integration |
| Requests | API communication |
| PyTorch | Deep learning experiments |
| Geneformer | Gene representation experiments |
| FAISS | Embedding similarity search |

## 🗂️ Repository Structure

```text
Gene-Annotation-and-Database-Validation/
│
├── notebooks/
│   ├── a.ipynb
│   ├── a1.ipynb
│   ├── f.ipynb
│   ├── n1.ipynb
│   └── adamson_novel_gene_discovery.ipynb
│
├── results/
│   ├── gene_availability.csv
│   ├── gene_database_source.csv
│   ├── genes_in_both.csv
│   ├── genes_not_available.csv
│   ├── genes_only_ncbi.csv
│   ├── genes_only_uniprot.csv
│   ├── not_available_genes.csv
│   ├── model_benchmark.csv
│   ├── unseen_gene_evaluation.csv
│   ├── CREB1_bio_vs_zero_comparison.csv
│   └── zero_shot_CREB1_results.csv
│
├── .gitignore
├── README.md
└── requirements.txt
```

*Note: Adjust the folder structure to match the actual files committed to the repository.*

## 📊 Analysis and Results

The project generates structured CSV outputs for:

- Gene availability across biological databases.
- Genes identified in both NCBI and UniProt.
- Genes found only in NCBI.
- Genes found only in UniProt.
- Genes not identified in the queried databases.
- Gene annotation and metadata comparisons.
- Computational gene candidate evaluation.

Database absence should not automatically be interpreted as evidence that a gene is biologically novel.

## 🧬 Novel Gene Candidate Exploration

An additional computational workflow explores:

- Geneformer-based representations.
- Autoencoder-based latent representations.
- UMAP dimensionality reduction.
- Leiden clustering.
- Candidate gene identification.
- NCBI Entrez annotation checks.
- AlphaFold structure availability.
- FAISS-based embedding similarity search.

These analyses generate computational candidate genes that require further biological validation.

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/aman13155/Gene-Annotation-and-Database-Validation.git
cd Gene-Annotation-and-Database-Validation
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate on Windows:

```powershell
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install scanpy anndata pandas numpy scipy
pip install mygene biopython requests tqdm
pip install scikit-learn matplotlib seaborn
pip install torch transformers gseapy
```

## 📁 Dataset

The project uses the Adamson Perturb-seq dataset.

Large `.h5ad` datasets and trained model checkpoints are not included directly in the standard Git repository. Obtain the datasets from their appropriate research sources and configure the notebook dataset paths before execution.

## 🔗 Biological Resources

- [NCBI Gene](https://www.ncbi.nlm.nih.gov/gene/)
- [NCBI Entrez](https://www.ncbi.nlm.nih.gov/books/NBK25501/)
- [MyGene.info](https://mygene.info/)
- [UniProt](https://www.uniprot.org/)
- [AlphaFold Protein Structure Database](https://alphafold.ebi.ac.uk/)

## 🚀 Future Work

- Improve cross-database gene identifier mapping.
- Integrate additional biological annotation resources.
- Develop reproducible gene validation workflows.
- Improve candidate gene prioritization.
- Perform experimental and literature-based validation of computational predictions.

## 👨‍💻 Author

**Aman Tarikere**

MCA Graduate | AI/ML and Bioinformatics Research

GitHub: [@aman13155](https://github.com/aman13155)

---

*This repository is intended for computational bioinformatics research, gene annotation, and biological database validation.*
