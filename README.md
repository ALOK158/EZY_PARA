# **Abstract Sentence Classification using NLP**

## **Overview**
This repository contains an NLP model designed to classify sentences in research abstracts into predefined categories such as **Objective, Methods, Results, Conclusion, etc.** The goal is to help researchers quickly skim through literature and dive deeper when necessary. The model is trained on the **[SkimLit dataset](https://github.com/Franck-Dernoncourt/pubmed-rct#readme)**.

## **Dataset: SkimLit**
[SkimLit](https://github.com/Franck-Dernoncourt/pubmed-rct#readme) is a dataset specifically designed for **scientific literature classification**, containing labeled sentences from biomedical abstracts. Each sentence is categorized based on the role it plays in the abstract, making it ideal for training models that facilitate **automatic summarization and information extraction**.

## **Model Description**
The model is built by concatenating a **character vectorization technique** and a **pretrained Universal Sentence Encoder model**. The character vectorization model uses **BiDirectional LSTM layers** instead of a 1D-CNN, providing enhanced contextual learning. The concatenated result of these two models is then passed through **dropout layers** to prevent overfitting. This architecture has shown to perform **slightly better than 1D-CNN-based models** for this task.

## **Features**
- ✅ **Pre-trained NLP model** for classifying abstract sentences
- ✅ **Multi-class classification** for different sections of abstracts
- ✅ **BiDirectional LSTM for character vectorization**
- ✅ **Universal Sentence Encoder for sentence embeddings**
- ✅ **Dropout layers for overfitting prevention**

