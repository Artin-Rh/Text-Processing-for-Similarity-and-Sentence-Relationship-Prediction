# Text-Processing-for-Similarity-and-Sentence-Relationship-Prediction


This repository contains a **Natural Language Processing (NLP) project** that aims to determine whether two given sentences (a question and an answer) are related. The project explores **two different deep learning approaches** for text similarity and relationship prediction.

## **Project Overview**
The dataset (`train.csv`) consists of:
- **qtext**: The question text.
- **atext**: The answer text.
- **label**: A binary indicator (1 if the answer is relevant to the question, 0 otherwise).

To address this problem, we implement two approaches:

### ** Task 1: Siamese Neural Network (TF-IDF + Contrastive Loss)**
- This model **converts text into numerical vectors** using **TF-IDF (Term Frequency-Inverse Document Frequency)**.
- A **Siamese Neural Network** is trained to learn a **distance function**, minimizing similarity for related pairs and maximizing it for unrelated pairs.
- This approach is **lightweight and effective for simple text similarity tasks**.

### ** Task 2: Transformer-Based Model (BERT for Sentence Relationship Prediction)**
- Instead of static embeddings, we **use a pre-trained Transformer model (e.g., BERT or DistilBERT)** to process question-answer pairs.
- The model **understands sentence relationships** by jointly encoding both the question and the answer.
- This approach is **more advanced** and **captures deeper semantic meaning** compared to the Siamese network.

---

## **Results & Performance**
| Model | Embedding Method | Training Approach | Context Awareness | Expected Performance |
|-------|----------------|------------------|-----------------|------------------|
| **Siamese NN** | TF-IDF | Contrastive Loss | Limited | Good for Simple Matching |
| **Transformer** | Pre-trained Model (BERT) | Fine-Tuning | High | Superior for Complex Text |

- The **Transformer model** significantly improves accuracy **by leveraging contextual embeddings**.
- The **Siamese Network** remains a strong baseline, particularly for smaller datasets or simpler tasks.

---

## **Future Improvements**
- Experiment with **different pre-trained Transformer models** (e.g., RoBERTa, ALBERT).
- Optimize the **Siamese Network** with **word embeddings** instead of TF-IDF.
- Explore **semi-supervised or unsupervised learning techniques** to improve generalization.

---

## **License**
This project is open-source and available under the [MIT License](LICENSE).

---

## **Contributing**
If you’d like to contribute:
1. **Fork the repository** and create a feature branch.
2. **Implement improvements** or **fix issues**.
3. **Submit a pull request** for review!

---

## **Contact**
For any questions or collaboration opportunities, feel free to reach out!

**Email**: [artin.rahmanian501@gmail.com](mailto:artin.rahmanian501@gmail.com)  
**LinkedIn**: [Artin-Rahmanian](https://www.linkedin.com/in/artin-rahmanian-24a058232) 


