# Applied Vision Transformer for CrisisMMD

This repository contains the research work for applying a Vision Transformer (ViT) to the CrisisMMD dataset with the goal of improving overall classification accuracy while preserving strong performance on rare and more severe classes.

## Overview

The project explores how a ViT-based approach can be used for multimodal disaster-related image classification, with particular emphasis on class imbalance and the need to retain sensitivity to critical events. The repository includes the main analysis notebook, exported HTML, report documents, and presentation materials.

## Repository contents

- `CrisisMMD_Final_Consolidated_Research_v3.ipynb` — primary notebook with experiments, analysis, and model exploration
- `CrisisMMD_Final_Consolidated_Research_v3.html` — rendered notebook version for convenient viewing in GitHub
- `CrisisMMD_Final_Research_Report_Enhanced_Previous_Version.docx` — research report
- `CrisisMMD_ViT_Research_Journey.pptx` — presentation deck summarizing the project
- `README.md` — project overview and usage guidance

## Research objective

This work evaluates whether a Vision Transformer can:

- achieve strong overall accuracy on CrisisMMD data
- maintain robustness for underrepresented but higher-impact disaster classes
- provide a useful research baseline for future work in crisis image classification

## Getting started

### 1. Clone the repository

```bash
git clone https://github.com/hozefa413/vit_research_crisisdataset_1677299.git
cd vit_research_crisisdataset_1677299
```

### 2. Create a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

If the notebook requires additional packages not yet listed in `requirements.txt`, install them as needed before running the analysis.

### 4. Open the notebook

Launch Jupyter and open the notebook:

```bash
jupyter notebook
```

Then open:

- `CrisisMMD_Final_Consolidated_Research_v3.ipynb`

## Suggested project workflow

1. Review the notebook for preprocessing and modeling steps.
2. Reproduce the experiments in a clean environment.
3. Validate the class imbalance handling and rare-class performance.
4. Extend the pipeline with additional augmentation, balancing, or tuning strategies.

## Data and environment notes

- This repository does not include the CrisisMMD dataset files directly.
- You will need access to the relevant dataset before running the notebook end-to-end.
- The code and analysis may require GPU acceleration depending on the configuration and notebook implementation.

## Contribution

Contributions, discussion, and suggestions are welcome. Please read `CONTRIBUTING.md` before opening issues or pull requests.

## License

This project is licensed under the MIT License. See `LICENSE` for details.

## Citation and context

This project is intended as a research artifact for applied vision transformer work on crisis-related image classification. It should be cited or referenced appropriately when used as a basis for further work.
