# Hindi Speech to English Text Translation System

## Objective
![image](https://github.com/user-attachments/assets/4ad7bb29-f225-4a26-8e29-1a866abfc95d)
## Pipeline
![image](https://github.com/user-attachments/assets/409d8e91-b196-47e3-b0f3-36ed0fe71345)

## System Overview

This system utilizes a two-step approach for efficient and modular speech-to-text translation. 

1. **Automatic Speech Recognition (ASR)**: The system processes Hindi audio input using an ASR model trained on the [OpenSLR Hindi dataset](https://www.openslr.org/103/), generating high-quality Hindi text transcriptions.
  
2. **Neural Machine Translation (NMT)**: The transcriptions are then translated into English using a neural machine translation (NMT) model trained on the [Bilingual Hindi-English Truncated Corpus](https://www.kaggle.com/datasets/umasrikakollu72/hindi-english-truncated-corpus).

Although the ASR and NMT models are trained independently, they are seamlessly integrated to form an end-to-end pipeline that combines speech recognition and translation into one unified process.

### Model Architecture

The sequence-to-sequence (seq2seq) model used in this pipeline is built with Long Short-Term Memory (LSTM) networks, which effectively manage long-term dependencies and mitigate the vanishing gradient problem. While the ASR model showed promising results despite resource constraints limiting the number of training epochs, the NMT model benefited from techniques like early stopping, dropout, and other regularization methods to prevent overfitting and improve performance on unseen data.


## Contributors
  [Ayan Maity](https://github.com/AyanMaity435601)
  
  [Debayan Datta](https://github.com/debayan-datta)
  
  [Debanjan Nanda](https://github.com/DebanjanNanda)
