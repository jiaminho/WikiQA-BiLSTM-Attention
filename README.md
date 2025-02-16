# WikiQA-BiLSTM-Attention
WikiQA: Open-Domain Question Answering using Bi-LSTM and Attention


# WikiQA: Open-Domain Question Answering using Bi-LSTM and Attention

## Overview
WikiQA is an open-domain question-answering system that leverages a Bi-LSTM model with an attention mechanism to identify correct answers from Wikipedia-based datasets. This project focuses on sequence modeling and embedding techniques to enhance answer extraction accuracy.

## Dataset
The model is trained and evaluated on the **Microsoft Research WikiQA Corpus**, which consists of question-sentence pairs derived from Bing query logs and linked to Wikipedia pages. Data preprocessing includes token labeling and sequence padding to improve model efficiency.

## Model Architecture
- **Word Embeddings:** Utilizes **FastText** to capture subword information and generate embeddings for out-of-vocabulary words.
- **Feature Extraction:** Incorporates **PoS tags, TF-IDF, and Named Entity Recognition (NER)** to improve contextual understanding.
- **Bi-LSTM with Attention:**
  - Separate Bi-LSTM encoders for questions and documents.
  - An attention mechanism enhances the model’s ability to focus on relevant tokens.
  - Output is determined using a softmax function to predict the start token of the correct answer.

## Training and Optimization
- **Loss Function:** CrossEntropyLoss for efficient classification.
- **Optimizer:** Adam optimizer selected for its adaptive learning rate and improved convergence.
- **Hyperparameter Tuning:**
  - Epochs: 10,000
  - Learning Rate: 0.1
  - Ablation studies confirm the optimal embedding and attention mechanisms.

## Performance Evaluation
Metrics used:
- **Precision, Recall, and F1-score** for assessing answer accuracy.
- Ablation studies show **FastText-only embeddings** and **Dot Product attention** provide the best performance.

## Contributors
- Abhishek Anand
- Shaikh Enamul Haque
- Jia Min Ho

## References
Refer to the report for detailed methodology and citations.

