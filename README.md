# BERT Sentiment Analysis on Twitter Data

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0-red)
![HuggingFace](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![Accuracy](https://img.shields.io/badge/Accuracy-74.3%25-green)

## Overview
Fine-tuned BERT transformer model for multi-class sentiment 
classification on Twitter data. Trained on 45,615 tweets to 
classify text as Positive, Negative, or Neutral.

## Results
| Metric | Score |
|--------|-------|
| Validation Accuracy | 74.3% |
| Test Accuracy | 67.62% |
| Dataset Size | 45,615 tweets |

## Confusion Matrix
![Confusion Matrix](confusion_matrix.png.png)

## Tech Stack
- Python 3.10
- PyTorch
- Hugging Face Transformers
- BERT (bert-base-uncased)
- Scikit-learn
- Google Colab (T4 GPU)

## Dataset
- **Source:** Cardiff NLP Twitter Eval Dataset
- **Task:** Sentiment Analysis
- **Classes:** Negative (0), Neutral (1), Positive (2)
- **Train:** 45,615 samples
- **Validation:** 2,000 samples
- **Test:** 12,284 samples

## Model Architecture
- Base: `bert-base-uncased`
- Classification Head: 3-class linear layer
- Max sequence length: 128 tokens
- Training epochs: 4
- Learning rate: 2e-5
- Batch size: 32

## Sample Predictions
Text: "I love this so much!"
Prediction: Positive (100% confidence)
Text: "This is the worst experience ever"
Prediction:  Negative (99.9% confidence)
Text: "Google interview went really well!"
Prediction:  Positive (100% confidence)

## How to Run
1. Open `Untitled0.ipynb` in Google Colab
2. Runtime → Change Runtime → T4 GPU
3. Run all cells in order
4. Training takes ~20 minutes on T4 GPU

## Author
**Arjith S R**  
B.E Computer Science (AI & ML)  
Sathyabama Institute of Science and Technology
