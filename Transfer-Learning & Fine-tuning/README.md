# NLP Fine-tuning & Transfer Learning Project

This project demonstrates fine-tuning and evaluating pretrained Transformer models on various NLP tasks, including sentiment analysis, commonsense reasoning, semantic similarity, and language inference.

---

## 1. Sentiment Analysis (Yelp Polarity)
- **Objective:** Fine-tune a RoBERTa model to classify Yelp reviews as positive or negative.
- **Methods:**
  - Data preprocessing using Hugging Face's `roberta-base` tokenizer.
  - Model fine-tuning with Hugging Face's `Trainer` API.
  - Hyperparameter tuning: learning rate, batch size, weight decay, and scheduler type.
- **Best Results:**  
  Achieved an accuracy of **94.67%** (linear scheduler, learning rate `5e-5`, batch size `16`).

**From this point forward, we deliberately avoid additional fine-tuning on our target datasets to highlight the power and limitations of transfer learning when directly using pretrained models.**

---

## 2. Commonsense Reasoning (PIQA Dataset)
- **Objective:** Evaluate pretrained multiple-choice models on commonsense reasoning tasks without additional fine-tuning.
- **Methods:**
  - Evaluated pretrained multiple-choice models (`BERT`, `RoBERTa`, `DeBERTa`) directly on the PIQA dataset.
- **Best Results:**  
  Best accuracy achieved by `Deberta_for_multiple_choice`: **74.3%**.
- **Note:**  
  Accuracy is lower compared to fine-tuned scenarios, highlighting the limitations yet impressive capability of pretrained models without additional training.

---

## 3. Semantic Similarity Evaluation (Truthful QA)
- **Objective:** Evaluate semantic similarity to identify optimal answers using pretrained Sentence Transformer embeddings.
- **Methods:**
  - Combined multiple-choice pretrained models with Sentence Transformer models (e.g., `all-mpnet-base-v2`, `stsb-roberta-base`).
  - Evaluated accuracy with a strict cosine similarity threshold (0.95).
- **Best Results:**  
  Highest accuracy: **44%** (baseline random accuracy ~25%).
- **Note:**  
  Performance demonstrates limitations but still significant improvement over chance, underscoring pretrained model strengths even without fine-tuning.

---

## 4. Language Understanding (Winogrande)
- **Objective:** Predict correct missing words using pretrained multiple-choice models without additional fine-tuning.
- **Methods:**
  - Transformed Winogrande dataset into a multiple-choice task.
  - Evaluated using pretrained models (`RoBERTa`, `DeBERTa`) directly.
- **Best Results:**  
  Best accuracy by `Deberta_for_multiple_choice`: **73%**.
- **Note:**  
  Results highlight the notable capability of transfer learning and pretrained models in understanding nuanced linguistic tasks, despite no further fine-tuning.

---

## Conclusions:
- Initial fine-tuning significantly boosts performance on specific NLP tasks.
- Subsequent experiments intentionally avoided fine-tuning, demonstrating both the impressive effectiveness and practical limitations of transfer learning alone.
- Results underline the importance of fine-tuning, yet also affirm the substantial benefits pretrained models offer even without further adjustments.
