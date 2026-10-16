# Automatic Image Tagging Using Machine Learning

## 1. Project Overview

This project aims to develop a machine learning system for automatically predicting multiple semantic labels from images using the NUS-WIDE dataset.

The task is **multi-label image classification**, meaning that a single image can be assigned multiple labels simultaneously.

The project considers 30 predefined image labels, including sky, clouds, person, water, animal, grass, buildings, and others.

## 2. Dataset

The project uses a stratified subset of the NUS-WIDE dataset containing 75,000 images and 30 labels.

| Dataset Split | Number of Images |
|---|---:|
| Training | 60,000 |
| Validation | 5,000 |
| Testing | 10,000 |
| **Total** | **75,000** |

The original train, validation, and test splits provided for the assignment will be preserved.

Each image may contain more than one positive label.

Due to the dataset size, image files are stored separately from the GitHub repository.

## 3. Project Objectives

- Explore and analyze the multi-label image dataset.
- Extract and compare different image feature representations.
- Implement baseline models and machine learning models.
- Develop and evaluate a Convolutional Neural Network (CNN).
- Optimize model hyperparameters and label-specific prediction thresholds.
- Analyze model performance, common errors, and limitations.
- Demonstrate automatic image tagging on an input image.

## 4. Methodology

The project is organized into the following stages:

1. **Data Preparation and EDA** — Validate dataset structure, analyze label frequencies, and investigate class imbalance.
2. **Feature Extraction** — Extract and compare at least two image feature representations.
3. **Model Development** — Implement baseline approaches, traditional machine learning models, and CNN-based approaches.
4. **Hyperparameter Tuning** — Select model configurations and optimize prediction thresholds using validation data.
5. **Evaluation** — Evaluate selected models using the predefined test set.
6. **Error Analysis** — Investigate incorrect predictions, class-specific weaknesses, and model limitations.

The experiments will include comparisons across at least three models and two feature representations, alongside the required baselines.

## 5. Evaluation Metrics

The main evaluation metrics are:

- **Macro-F1 (Primary Metric):** Evaluates performance equally across all labels.
- **Micro-F1:** Measures overall multi-label prediction performance using aggregated true positives, false positives, and false negatives.
- **Subset Accuracy:** Measures the proportion of images for which all 30 predicted labels are exactly correct.

## 6. Technologies

- Python
- Google Colab
- GitHub
- Google Drive
- NumPy and Pandas
- Matplotlib and Seaborn
- Scikit-learn
- PyTorch and Torchvision

## 7. Repository Structure

```text
MachineLearning_Project/
├── data/               # Dataset documentation and placeholders
├── notebooks/          # EDA and experiment notebooks
├── src/                # Reusable Python source code
├── results/            # Experiment summaries and selected results
├── reports/            # Project report and presentation
├── .gitignore
├── requirements.txt
└── README.md
```

Large datasets and trained model checkpoints are excluded from Git version control.

## 8. Reproducibility

The experiments will use the predefined dataset splits, documented preprocessing procedures, reproducible random seeds, and recorded package versions.

Training and validation data will be used for model development and tuning. Test data will be reserved for final evaluation.

The final submission will include a reproducible notebook, dependency information, test prediction probabilities, label-specific thresholds, an experiment comparison, and a project report.

## 9. Project Status

**Current Stage: Phase 2 — Feature Extraction**

### Completed
- Repository structure and initial setup.
- Google Colab environment and Google Drive integration.
- Dataset loading and validation of the predefined splits.
- Image integrity verification of all 75,000 images.
- Exploratory Data Analysis (EDA), including:
  - Label distribution.
  - Class imbalance analysis.
  - Labels per image.
  - Label co-occurrence.
- Upload of the Phase 1 notebook to GitHub.

### In Progress
- Feature extraction using handcrafted and pretrained CNN features.

### Upcoming
- Baseline models and multi-label classification experiments.
- CNN development and hyperparameter tuning.
- Model evaluation and error analysis.
- Final report, test predictions, thresholds, and live demonstration.

## 10. Quick Start (Google Colab)

1. Open `notebooks/ML_Project.ipynb` in Google Colab.
2. Connect Google Drive containing the provided NUS-WIDE dataset archive and CSV files.
3. Check the dataset paths in the setup cells.
4. Run the environment setup and dataset preparation cells.
5. Verify that all 75,000 images are available and readable.
6. Run the notebook sections required for the intended experiment.

**Note:** The image dataset and large model checkpoints are not stored in this repository. The dataset must be obtained separately, and the local Google Drive paths must be configured before running the notebook.

Model training, evaluation results, and the interactive prediction demonstration will be added as development progresses.
