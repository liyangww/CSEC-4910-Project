## Project Overview

This repository contains all the deliverables for my senior project in Computer Science and Economics:

- The LaTeX thesis and all figures/tables.
- Jupyter notebooks for data exploration, modeling, and evaluation.
- All CSV outputs, raw and processed datasets used in the analysis.

## Repository Structure

- **thesis/**  
    Compile `main.tex` in the folder to build the thesis PDF from source files. A copy of the compiled PDF is also included for convenience.

- **notebooks/**  
  Jupyter notebooks for each stage:
  - `01_data_exploration.ipynb`: Data loading and initial analysis.
  - `02_clustering_methods.ipynb`: Clustering-based regime identification.
  - `03_markov_switching.ipynb`: Markov-switching model analysis.
  - `master.ipynb`: Aggregates results and generates summary figures/tables.
- **data/**  
  - `macro_dataset.csv`: Preprocessed macroeconomic panel.
  - `regime_assignments_all_methods.csv`: Regime assignments (hard/soft).
  - `regime_evaluation_summary.csv`: Evaluation metrics for all methods.

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/liyangww/CSEC-4910-Project.git
   cd CSEC-4910-Project
   ```

2. **Set up the Python environment:**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```
   - Tested with Python 3.13. All dependencies are pinned in `requirements.txt`.

3. **Working with Notebooks:**
   - Activate the virtual environment.
   - Launch Jupyter:
     ```bash
     jupyter lab
     ```
   - Open notebooks from the `notebooks/` directory.
   - Data files are included; all paths are relative to the repository root.

4. **Building the Thesis:**
   - Navigate to the `thesis/` directory:
     ```bash
     cd thesis
     latexmk -pdf main.tex
     ```
   - The compiled PDF (`main.pdf`) is versioned for convenience.

## Best Practices

- Use the provided `.gitignore` to avoid committing virtual environments, OS files, and LaTeX build artifacts.
- All code and data are self-contained; no external downloads required.
- No AI-generated content or markers are present in the thesis or notebooks.

## License

This project is for academic use only. Please contact the author for reuse or collaboration.
