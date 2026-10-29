# 🛡️ Web Phishing Detection

A machine learning model that classifies websites as **legitimate** or **phishing** using URL structure and page-level features.

## Results

| Model | Accuracy |
|-------|----------|
| **Random Forest** | **96.5%** |

Precision and recall of 0.96–0.97 on both classes (balanced test set of 2,286 URLs).

## Dataset

11,430 URLs with 89 features, including URL length, special-character counts, domain and host properties, and page-content signals. Balanced between legitimate and phishing sites.

## Workflow

1. Exploratory data analysis and class-distribution checks
2. Label encoding and feature scaling
3. Model training and comparison with Scikit-learn classifiers and a Keras neural network
4. Evaluation with accuracy, classification report and confusion matrix
5. Interactive Gradio demo for testing predictions

## Tech stack

Python · Pandas · Scikit-learn · TensorFlow/Keras · NLTK · Matplotlib · Seaborn · Gradio

## Run

```bash
git clone https://github.com/arunak451/web-phishing-detection.git
pip install jupyter pandas numpy scikit-learn tensorflow nltk matplotlib seaborn gradio
jupyter notebook web_phishing_proj.ipynb
```

The notebook expects `dataset_phishing.csv` (originally run on Google Colab from `/content/`).
