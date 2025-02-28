# Quora-Question-Pairs

**Question Pair Similarity Classification**

## Project Overview
This project focuses on classifying duplicate question pairs using the **Quora Question Pairs** dataset. The goal is to identify whether two given questions are semantically identical using various machine learning and deep learning models.

## Dataset
Dataset Source: [Kaggle Quora Question Pairs](https://www.kaggle.com/c/quora-question-pairs)

### Dataset Description
- Total Samples: 404,287
- Features:
  - Question1
  - Question2
  - is_duplicate (Target Variable)
- Target Distribution:
  - Non-Duplicate: 63.08%
  - Duplicate: 36.92%

## Project Structure
```
|-- data/               # Dataset Files
|-- notebooks/          # Jupyter Notebooks
|-- models/             # Saved Models
|-- src/                # Source Code
|-- README.md           # Project Overview
|-- requirements.txt    # Dependencies
```

## Dependencies
Install the required dependencies using:
```bash
pip install -r requirements.txt
```

## Models Implemented
- Logistic Regression (Baseline)
- Artificial Neural Network (ANN)
- Long Short-Term Memory (LSTM)

### Performance Comparison
| Model       | Accuracy | Precision | Recall | F1-Score | AUC-ROC |
|------------|----------|----------|-------|----------|---------|
| Logistic Regression | 63.08% | - | - | - | - |
| ANN        | 90.04%   | 86.19%   | 86.97% | 86.58%   | 95.95%  |
| LSTM       | **92.16%** | **88.14%** | **91.00%** | **89.55%** | **96.97%** |

## How to Run
1. Clone the repository:
```bash
git clone https://github.com/username/project-name.git
```
2. Navigate to the project directory:
```bash
cd project-name
```
3. Run the Jupyter Notebooks for model training and evaluation.

## Results
The **LSTM model** achieved the highest performance with an **accuracy of 92.16%** and **AUC-ROC of 96.97%**.

