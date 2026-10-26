# Applied Vision Transformer for CrisisMMD

This repository contains a research project on applying a Vision Transformer (ViT) to the CrisisMMD dataset. The goal is to evaluate whether a transformer-based model can achieve strong overall classification accuracy while still handling rarer, more serious disaster-related classes effectively.

## Project description

This project explores how a ViT-based approach can be used for crisis-related image classification. The work is motivated by the need to balance strong overall performance with robustness on underrepresented but high-impact categories that are often critical in emergency response applications.

The main research focus is on understanding whether Vision Transformers can:

- achieve strong overall accuracy on CrisisMMD data
- maintain reliable performance for minority but important disaster classes
- provide a useful research baseline for future work in crisis image analysis

## Language composition

This repository is primarily composed of:

- HTML: 54.1%
- Jupyter Notebook: 45.9%

This composition reflects the project’s notebook-driven research workflow and the inclusion of a rendered HTML version for easier viewing in GitHub.

## Overview

The project investigates multimodal disaster-related image classification using a ViT architecture. In emergency contexts, models must not only perform well on frequent classes but also remain useful for rare but operationally important situations. This research examines that balance and provides a foundation for further study in crisis-related computer vision.

## Repository contents

- `CrisisMMD_Final_Consolidated_Research_v3.ipynb` — main notebook with preprocessing, experimentation, and analysis
- `CrisisMMD_Final_Consolidated_Research_v3.html` — rendered notebook output for convenient viewing in GitHub
- `CrisisMMD_Final_Research_Report_Enhanced_Previous_Version.docx` — research report
- `CrisisMMD_ViT_Research_Journey.pptx` — presentation deck summarizing the project
- `README.md` — project overview and usage guidance
- `docs/` — supporting documentation folder

## Research objective

This work evaluates whether a Vision Transformer can:

- achieve strong overall performance on crisis-related image data
- maintain robustness for underrepresented but high-impact disaster classes
- serve as a meaningful baseline for future research in visual crisis analysis

## Dataset context

The project uses the CrisisMMD dataset, which is designed for disaster-related classification tasks in crisis informatics and emergency-response research. The dataset presents class imbalance challenges, making it suitable for studying model performance under real-world imbalance conditions.

## Setup

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

### 3. Install the required Python packages

There is no `requirements.txt` file included in this repository. Install the dependencies needed for the notebook manually, typically including packages such as:

```bash
pip install jupyter numpy pandas matplotlib scikit-learn opencv-python torch torchvision
```

If the notebook uses additional libraries, install them as needed before running the analysis.

### 4. Open the notebook

Start Jupyter and open the notebook:

```bash
jupyter notebook
```

Then open:

- `CrisisMMD_Final_Consolidated_Research_v3.ipynb`

## Suggested workflow

1. Review the notebook to understand the preprocessing and modeling pipeline.
2. Reproduce the experiments in a clean environment.
3. Evaluate both overall performance and sensitivity to rare, severe classes.
4. Extend the project with alternative augmentation, balancing, or transformer tuning strategies.

## Data and environment notes

- This repository does not include the CrisisMMD dataset files directly.
- You must obtain access to the dataset before running the notebook end-to-end.
- The project may require GPU acceleration depending on the environment and implementation details.
- The repository is intended for research exploration and academic experimentation.

## Project significance

This work contributes to the broader study of modern vision models in humanitarian and emergency settings. The central question is not only whether the model can achieve high aggregate accuracy, but also whether it can remain useful when class distributions are imbalanced and rare classes have greater real-world importance.

## Contribution

Contributions, suggestions, and discussion are welcome. If you want to improve or extend the work, feel free to open an issue or submit a pull request with experiments, analysis, or documentation updates.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Citation and context

This project is intended as a research artifact for applied Vision Transformer work on crisis-related image classification. It should be cited or referenced appropriately when used as a basis for future study or publication.

## Summary

This repository provides a research notebook and supporting materials for applying a Vision Transformer to the CrisisMMD dataset, with a focus on balancing overall accuracy and performance on rarer, more serious disaster classes.
