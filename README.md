# Applied Vision Transformer for CrisisMMD

This repository contains a research project focused on applying Vision Transformer (ViT) models to the CrisisMMD dataset. The goal is to investigate whether transformer-based image classification can achieve strong overall accuracy while maintaining reliable performance on rarer but more critical damage classes.

The project is designed around a practical research question: in disaster-response and crisis informatics settings, a model should not only perform well on common classes, but also remain useful for minority classes that may represent higher-severity situations.

## Project summary

The project studies how modern deep learning architectures can support crisis image analysis for damage classification. In particular, it explores the application of Vision Transformers to images from the CrisisMMD dataset and evaluates trade-offs between:

- overall classification accuracy
- balanced accuracy
- macro-F1 performance
- sensitivity to rare and severe classes
- model generalization and practical usability

The repository includes a research notebook, rendered analysis output, supporting reports, and presentation materials. It is intended primarily as a research artifact and an exploratory benchmark for transformer-based disaster-damage classification.

## Research objective

This work examines whether a ViT-based model can:

- achieve strong performance on crisis-related image data
- generalize effectively across diverse disaster scenarios
- maintain useful recall for underrepresented but important classes
- serve as a strong baseline for future crisis image analysis work

## Dataset and task

The project uses the CrisisMMD dataset, which is a disaster-related dataset commonly used for crisis informatics and humanitarian response research.

The task is image-based disaster-damage classification, with an emphasis on distinguishing damage severity levels. In real-world emergency settings, poor performance on rarer but more serious classes can be especially costly, so the project pays careful attention to class imbalance and metric selection.

## Why this project matters

In crisis monitoring and emergency response applications, image classification can help identify damage severity, affected infrastructure, and event impact. However, many disaster datasets are imbalanced and skewed toward more frequent classes. This project focuses on whether transformer-based models can provide a good balance between headline accuracy and reliability for the rarer cases that may matter most operationally.

## Language composition

This repository is primarily composed of:

- HTML: 54.1%
- Jupyter Notebook: 45.9%

This composition reflects the notebook-driven research workflow and the inclusion of an HTML-rendered notebook for easier browsing on GitHub.

## Repository structure

- `CrisisMMD_Final_Consolidated_Research_v3.ipynb` — main research notebook containing preprocessing, modeling, experiments, and evaluation results
- `CrisisMMD_Final_Consolidated_Research_v3.html` — rendered version of the notebook for convenient viewing in GitHub
- `CrisisMMD_Final_Research_Report_Enhanced_Previous_Version.docx` — final research report in document form
- `CrisisMMD_ViT_Research_Journey.pptx` — presentation deck summarizing the project narrative and findings
- `README.md` — repository overview and setup instructions
- `requirements.txt` — Python package dependencies required to run the notebook
- `docs/` — supporting project documentation (if present in the repository)

## Project workflow

The repository is structured around a research workflow that typically includes:

1. dataset loading and inspection
2. annotation and image validation
3. preprocessing and label preparation
4. model experimentation with transformer-based architectures
5. evaluation using classification metrics
6. comparison of model configurations and training strategies
7. documentation of findings and final conclusions

## Expected environment

The project is intended for a Python-based experimental environment, typically with:

- Python 3.9+
- Jupyter Notebook or JupyterLab
- optional GPU acceleration for faster training
- PyTorch-based model training workflow

## Setup instructions

### 1. Clone the repository

```bash
git clone https://github.com/hozefa413/vit_research_crisisdataset_1677299.git
cd vit_research_crisisdataset_1677299
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

On macOS/Linux:

```bash
source .venv/bin/activate
```

On Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

Install the required packages using the repository's dependency file:

```bash
pip install -r requirements.txt
```

If you are working in a notebook environment that does not yet have dependencies installed, you can also install the most common packages manually:

```bash
pip install jupyter pandas numpy matplotlib seaborn scikit-learn pillow torch torchvision timm transformers mlflow
```

### 4. Launch Jupyter

```bash
jupyter notebook
```

Then open:

- `CrisisMMD_Final_Consolidated_Research_v3.ipynb`

## Data requirements

This repository does not include the CrisisMMD dataset files directly. To run the notebook end-to-end, you must obtain the dataset separately and place it in an accessible local directory as expected by the notebook's preprocessing code.

Important notes:

- the dataset is not bundled with the repository
- image files and annotation files need to be available locally
- some notebook execution may require adjusting dataset paths
- GPU acceleration is strongly recommended for model training and experimentation

## Notebook usage

The main notebook is the central artifact of this repository. It is intended as a consolidated record of the research process and contains the implementation used to explore the ViT-based approach.

Recommended sequence:

1. open the notebook in Jupyter
2. review the environment setup cells
3. confirm all dependencies are installed
4. validate dataset paths and file access
5. run the analysis pipeline and experiment cells
6. compare findings across validation and test metrics

## Dependencies and tools

The project uses a scientific Python stack and deep learning tooling, including:

- Python
- Jupyter
- NumPy
- pandas
- Matplotlib
- Seaborn
- scikit-learn
- Pillow
- PyTorch
- TorchVision
- timm
- transformers
- MLflow

## Troubleshooting

### Missing package errors

If you encounter `ModuleNotFoundError`, reinstall the environment from `requirements.txt`:

```bash
pip install -r requirements.txt
```

### GPU not detected

Ensure that the correct CUDA-enabled PyTorch build is installed for your system. Some environments may need a GPU-enabled installation or a different CUDA version.

### Dataset path errors

Check that the CrisisMMD files are stored in the expected directory structure used by the notebook. If the notebook refers to a local dataset path, update it before running the cells.

### Notebook execution issues

If the notebook crashes or slows down, verify:

- Python version compatibility
- installation of deep learning dependencies
- dataset access and path correctness
- GPU availability
- memory and runtime constraints

## File details

The repository includes both executable research materials and supporting documents:

- the notebook provides the main technical implementation
- the HTML file is a rendered notebook snapshot
- the Word file offers a report-style narrative
- the PPTX file summarizes the research journey and findings

## Academic context

This project is intended as a research artifact for applied Vision Transformer work on crisis-related image classification. It can be used as a foundation for further experimentation in areas such as:

- class imbalance handling
- stronger data augmentation
- domain adaptation
- transfer learning
- rare-class optimization
- operational deployment analysis

## Contribution and extension

This repository is suitable for experimentation and future development. Improvements may include:

- stronger baseline comparisons
- ablation studies
- better imbalance handling
- hyperparameter tuning
- model benchmarking
- reproducible training scripts and pipelines

## Notes

- This repository is centered on research and experimentation rather than a packaged software library.
- The model and training outputs are intended for academic and exploratory use.
- Dataset access and environment setup are required before the notebook can be executed fully.

## Summary

This repository provides a research-focused implementation and supporting materials for applying Vision Transformers to disaster-damage classification using CrisisMMD. The work is especially relevant for scenarios where strong aggregate accuracy must be balanced with reliable performance on rarer, more severe classes.

