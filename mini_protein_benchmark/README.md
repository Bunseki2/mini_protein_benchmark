
# Mini-Protein Design Benchmark: ESM-2 vs ProteinMPNN vs ProtT5

This project benchmarks three modern protein language models for de novo generation of mini-protein sequences (40–60 residues):

- [ESM-2](https://github.com/facebookresearch/esm)
- [ProteinMPNN](https://github.com/dauparas/ProteinMPNN)
- [ProtT5](https://github.com/agemagician/ProtTrans)

We compare generated sequences in terms of:
- **Structure confidence** (pLDDT via AlphaFold2/ColabFold)
- **Foldability**
- **Sequence diversity**
- **Physicochemical features**

## 📦 Tools Used
- ESM-2 (Facebook Research)
- ProteinMPNN (Baker Lab)
- ProtT5 (Hugging Face Transformers)
- AlphaFold2 (via ColabFold batch)
- Python, Biopython, Pandas, Matplotlib

## 🧪 Project Layout
- `notebooks/`: Core generation, prediction, and analysis notebooks
- `scripts/`: Utility scripts for batch AlphaFold prediction and metric computation
- `data/`: Stores sequences, structures, and metrics
- `results/`: Final summary plots and tables



[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bunseki2/mini_protein_benchmark/blob/main/notebooks/01_generate_sequences_ESM2.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bunseki2/mini_protein_benchmark/blob/main/notebooks/02_generate_sequences_ProtT5.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bunseki2/mini_protein_benchmark/blob/main/notebooks/03_generate_sequences_ProteinMPNN.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bunseki2/mini_protein_benchmark/blob/main/notebooks/04_structure_predictionColabFold.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bunseki2/mini_protein_benchmark/blob/main/notebooks/05_analysis.ipynb)

## 🚀 How to Run
```bash
conda env create -f environment.yml
conda activate protein-benchmark

