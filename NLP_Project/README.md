# Multi-Architecture Semantic Analysis 

### Sentence Representation Learning with Neural Models

This project serves as a comprehensive benchmark for evaluating various neural architectures in the domain of **Sentence Representation Learning**. By implementing models ranging from simple statistical baselines to advanced recursive structures, it explores how to extract high-dimensional semantic features from text for downstream sentiment classification.

## 🚀 Key Highlights

* **Architecture Diversity**: Implements and compares 10+ variations of neural models including CBoW, LSTM, and Tree-LSTM.
* **Scientific Rigor**: Includes structured performance analysis focusing on model behavior across different linguistic complexities (e.g., sentence length).
* **Advanced NLP Techniques**: Explores recursive neural networks that leverage the inherent tree structure of human language.

## 🛠 Tech Stack

* **Language**: Python 3.x
* **Deep Learning**: PyTorch
* **Natural Language Processing**: NLTK (Tree parsing & visualization)
* **Data Analysis**: NumPy, Matplotlib

## 📊 Dataset: Stanford Sentiment Treebank (SST)

Unlike standard sentiment tasks, this project utilizes the **SST**, which provides:

* **Granular Sentiment Mapping**: Labels for every constituent node in the binary tree, not just the full sentence.
* **Structural Complexity**: Allows for testing models that utilize the recursive nature of syntax.

## 🏗 Implemented Architectures

The project explores the evolution of sentence representation through:

1. **Linear Baselines**:
* **BoW / CBoW**: Establishing a performance floor.
* **Deep CBoW**: Investigating the impact of non-linear hidden layers with pre-trained embeddings.


2. **Sequential Modeling**:
* **LSTM**: Capturing temporal dependencies and long-distance information flow.
* **Mini-batched & Tuned LSTM**: Optimizing training efficiency and hyperparameter sensitivity.


3. **Recursive Modeling (State-of-the-Art)**:
* **Tree-LSTM**: A specialized architecture that processes data according to its grammatical structure.
* **Child-Sum Tree LSTM**: Handling arbitrary numbers of children in a recursive framework.



## 📈 Performance Evaluation

The models were evaluated based on their accuracy relative to **Sentence Length**. Key findings include:

* **Depth Matters**: Deep CBoW significantly outperforms simple BoW by capturing non-linear feature interactions.
* **Sequence vs. Structure**: While LSTM performs well on linear sequences, **Tree-LSTM** variants demonstrate superior robustness in capturing fine-grained sentiment within complex syntactic structures.

## 📂 Repository Structure

* `NLP_Project_Sentence_Analysis.ipynb`: Main notebook containing data pipeline, model implementation, and evaluation.

## 💻 Quick Start

1. **Clone the repository**:
```bash
git clone (https://github.com/leah168/project-llm-foundations/tree/c6a632df3cfbcf187eea7b938d33b8c43fd54741/NLP_Project)

```


2. **Install dependencies**:
```bash
pip install torch nltk numpy matplotlib

```


3. **Run the analysis**:
Execute the cells in `NLP_Project_Sentence_Analysis.ipynb` to download data and train models.

---

