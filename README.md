BookLensX – NLP & Data Science Project

BookLensX is an advanced multi-task Natural Language Processing (NLP) system developed to enhance the understanding and interaction with book titles. This project integrates three core NLP tasks into a unified pipeline:

Rating Prediction: Predicts the rating of a book based on its title.

Genre Classification: Classifies the book into its appropriate genre.

Title Generation: Generates a descriptive title for a book.

Utilizing state-of-the-art models like BERT and T5, BookLensX employs shared encoders with task-specific output layers, optimizing performance across all tasks. The training process incorporates a joint multi-task loss function to ensure cohesive learning.

A multi-task NLP system for book title rating prediction, genre classification, and intelligent title generation using BERT, T5, and other large language models.

---

## Project Overview

**BookLensX** integrates three natural language processing tasks into a single multi-task learning pipeline:
- **Rating Prediction** (regression)
- **Genre Classification** (multi-class classification)
- **Title Generation** (sequence-to-sequence generation)

The system uses shared encoders (e.g., BERT, RoBERTa) with task-specific output layers. T5 or BART models are used for the generation task. The training process uses a joint multi-task loss function.

---

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- BERT/BART/T5
- Scikit-learn
- Jupyter Notebook
- Google Colab or Kaggle for GPU training

---

## Project Structure (Planned)
