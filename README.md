# Macro Regime Evaluation (Senior Thesis)

## Overview
- Comparative study of clustering-based and Markov-switching models for U.S. macro regime identification using the FRED-MD panel (1962–2025).
- Includes LaTeX thesis, analysis notebooks that recreate figures/tables, and CSV outputs used for evaluation.

## Repository Layout
- `thesis/` — LaTeX sources and figures; `main.tex` builds the thesis (`main.pdf` currently present).
- `notebooks/` — Jupyter notebooks (`01_data_exploration.ipynb`, `02_clustering_methods.ipynb`, `03_markov_switching.ipynb`, `master.ipynb` aggregator).
- `data/` — Prepared inputs/outputs: `macro_dataset.csv` (preprocessed panel), `regime_assignments_all_methods.csv` (hard/soft regimes), `regime_evaluation_summary.csv` (scored metrics).
- `venv/` — Local virtual environment (ignored by Git; do not commit).

## Setup
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```
- Tested with Python 3.13; packages pinned in `requirements.txt`.

## Working with Notebooks
- Activate the env, then launch `jupyter lab` (or `jupyter notebook`) and open files under `notebooks/`.
- Data files are already included; paths in notebooks assume repository root as the working directory.

## LaTeX Build
- From `thesis/`, run `latexmk -pdf main.tex` (or your TeX engine of choice).
- `.gitignore` excludes common build artifacts; keep `main.pdf` if you want the compiled document versioned.

## Preparing for GitHub
- Use the provided `.gitignore` to avoid committing `venv/`, OS cruft, and LaTeX intermediates.
- No AI-assistance markers were found in text sources or notebook code cells; images are static figure outputs.
