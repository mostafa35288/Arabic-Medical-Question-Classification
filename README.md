# Arabic Medical Question Classification

Classifying Arabic medical questions into 5 medical specialties with deep learning, on the MAQA dataset.

## Dataset
[MAQA dataset](https://www.kaggle.com/datasets/manarm7md/maqa-dataset) (downloaded with kagglehub). Questions are classified into 5 specialties.

## Approach
- Arabic text preprocessing, Keras Tokenizer and padded sequences.
- Trained and compared five architectures on the same split: RNN, CNN, BiRNN, LSTM, GRU.

## Results (test accuracy)
| Model | Test accuracy |
|-------|---------------|
| CNN | 87.5% |
| LSTM | 85.9% |
| GRU | 84.5% |
| RNN | 80.6% |
| BiRNN | 80.7% |

The CNN performed best on the held-out test set (8,500 questions).

## Files
- `NTI-Day6_task1.ipynb` - full pipeline: data loading, EDA, preprocessing, all five models, evaluation.

## Stack
Python, TensorFlow/Keras, pandas, scikit-learn, matplotlib, seaborn. Built during NTI Summer Training (NLP).
