# Research Summary

## Overview

This project studies disaster-damage classification using the CrisisMMD dataset and evaluates several Vision Transformer-based approaches. The research is motivated by the need to achieve strong overall classification accuracy while retaining robust detection of rarer and more severe disaster classes.

## Dataset

The dataset used for the study is CrisisMMD `image_damage`.

- Total images: 3,463
- Little/no damage: 2,166
- Mild damage: 823
- Severe damage: 474
- Training split: 2,077
- Validation split: 693
- Test split: 693
- Split strategy: stratified image-level split with seed 42

## Task definition

The task is a 3-class image classification problem:

- `little_or_no_damage`
- `mild_damage`
- `severe_damage`

This is a class-imbalanced problem, which makes the model selection process particularly sensitive to metrics such as Macro-F1 and balanced accuracy, not just overall accuracy.

## Models evaluated

The project compared multiple model families and configurations:

- ViT Base
- ConViT Tiny
- DINOv2 Base
- DINOv2 learning-rate sweep and fine-tuning experiments
- Different head designs and loss settings
- Controlled augmentation experiments

The final selected model was a DINOv2-based configuration using a convolutional head and focal loss, selected with validation Macro-F1 as the main criterion.

## Final selected run

- Run name: `E07_Aug_Realistic_FocalG1`
- MLflow run id: `bc6de0c9e94a4addbf10c27936d98a4a`

## Final results

### Validation performance

- Validation accuracy: 71.72%
- Validation balanced accuracy: 65.60%
- Validation Macro-F1: 64.18%

### Test performance

- Test accuracy: 69.41%
- Test balanced accuracy: 61.30%
- Test Macro-F1: 59.78%
- Test weighted F1: 70.23%

## Conclusion

Across the notebook, the HTML export, the report, and the presentation, the project consistently concludes that a ViT/DINOv2-based approach is the most promising choice for CrisisMMD disaster damage classification. The research indicates that the model can reach competitive overall performance while maintaining stronger handling of the rarer but more critical severe-damage classes. However, the project also notes that the problem remains challenging and requires careful validation due to class imbalance and event-level data leakage risks.

## Relevant files

- `CrisisMMD_Final_Consolidated_Research_v3.ipynb`
- `CrisisMMD_Final_Consolidated_Research_v3.html`
- `CrisisMMD_Final_Research_Report_Enhanced_Previous_Version.docx`
- `CrisisMMD_ViT_Research_Journey.pptx`

