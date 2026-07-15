# 🚀 Pep-Learning

> **Placement preparation repository** — A collection of projects, implementations, notes, and practice problems covering **Generative AI**, **Machine Learning**, **Neural Networks**, **Data Structures & Algorithms**, and more.

---

## 📌 About

This repository serves as a centralized hub for all my placement training work. Each topic contains hands-on implementations, coding exercises, course notes, and real-world mini-projects built during placement classes.

**Goal:** Build a strong, demonstrable portfolio covering the core CS & AI/ML concepts expected in technical interviews and placement rounds.

---

## 📂 Repository Structure

```
Pep-Learning/
│
├── 📁 NN/                                         # Neural Network implementations
│   ├── perceptron.ipynb                            # Single-layer Perceptron
│   ├── perceptron_for_multiclass.ipynb             # Multi-class Perceptron
│   ├── ANN.ipynb                                   # Artificial Neural Network
│   ├── CNN.ipynb                                   # Convolutional Neural Network
│   ├── cnn-implementation-from-scratch.ipynb       # CNN built from scratch
│   ├── rnn-from-scratch.ipynb                      # RNN built from scratch
│   ├── RNN_PT.ipynb                                # RNN PyTorch implementation
│   ├── RNN_tensorflow_implementation.ipynb         # RNN TensorFlow implementation
│   ├── CNN-from-scratch/                           # CNN scratch implementation (with dataset)
│   │   ├── digits-mnist-classification-using-cnn.ipynb
│   │   ├── train.csv
│   │   ├── test.csv
│   │   └── sample_submission.csv
│   └── data/                                       # MNIST raw data
│
├── 📁 NLP/                                         # Natural Language Processing
│   ├── NLP_basics.ipynb                            # NLP Basics implementation
│   ├── nlp-basics.ipynb
│   ├── spam.csv
│   └── twitter_mask4.jpeg
│
├── 📁 Notes/                                       # Course notes (PDFs)
│   ├── Intro.pdf
│   ├── Artificial Intelligencr.pdf
│   ├── Activation Functions.pdf
│   ├── Neural Networks.pdf
│   ├── Regression.pdf
│   ├── Classification.pdf
│   ├── Classification-DEcesion_tree.pdf
│   ├── Decision Tree Regressor.pdf
│   ├── Clustering.pdf
│   ├── Encoding.pdf
│   ├── Model Evaluation.pdf
│   └── CIFAR-10 Dataset.pdf
│
├── 📁 GEN-AI/                                      # Generative AI implementations (BERT, RAG, etc.)
│
├── 📁 OLLAMA_APP/                                  # Standalone Ollama-based App (UV-managed)
│
├── mnist-dataset-cnn-implementation.ipynb          # MNIST CNN (Kaggle notebook)
├── bhagavad-gita-in-english-source-file-2.pdf      # Source document for RAG pipelines
├── requirements.txt                                # Python dependencies
├── .gitignore
└── README.md
```

---

## 🧠 Topics Covered

### 1. Neural Networks / Deep Learning

| Project | Description | Tech | Status |
|---------|-------------|------|--------|
| [Perceptron](NN/perceptron.ipynb) | Single-layer perceptron implementation | Python, NumPy | ✅ Done |
| [Multi-class Perceptron](NN/perceptron_for_multiclass.ipynb) | Perceptron for multi-class classification | Python, NumPy | ✅ Done |
| [ANN](NN/ANN.ipynb) | Artificial Neural Network implementation | Python, TensorFlow | ✅ Done |
| [CNN](NN/CNN.ipynb) | Convolutional Neural Network | TensorFlow, Keras | ✅ Done |
| [CNN from Scratch](NN/cnn-implementation-from-scratch.ipynb) | CNN implementation without high-level APIs | Python, NumPy | ✅ Done |
| [RNN from Scratch](NN/rnn-from-scratch.ipynb) | RNN built from scratch | Python, NumPy | ✅ Done |
| [RNN PyTorch](NN/RNN_PT.ipynb) | RNN PyTorch implementation | Python, PyTorch | ✅ Done |
| [RNN TensorFlow](NN/RNN_tensorflow_implementation.ipynb) | RNN TensorFlow implementation | Python, TensorFlow | ✅ Done |
| [MNIST CNN (Kaggle)](mnist-dataset-cnn-implementation.ipynb) | CNN for handwritten digit classification (0–9) | TensorFlow, Keras, Scikit-learn | ✅ Done |
| [MNIST Classification](NN/CNN-from-scratch/digits-mnist-classification-using-cnn.ipynb) | MNIST digit classification with CNN | TensorFlow, Keras | ✅ Done |

<details>
<summary><b>📊 MNIST CNN (Kaggle) — Key Results</b></summary>

- **Architecture:** Conv2D(32) → MaxPool2D → Flatten → Dense(128) → Dense(10, Softmax)
- **Training Accuracy:** 99.9%
- **Validation Accuracy:** 98.6%
- **Total Parameters:** 693,962
- **Optimizer:** Adam | **Loss:** Sparse Categorical Crossentropy
- **Epochs:** 10 | **Batch Size:** 32

</details>

---

### 2. Course Notes (PDFs)

#### 📚 Automated Course Notes Sync

`Notes/` is kept in sync with [alenso0/LPU-GenAi](https://github.com/alenso0/LPU-GenAi)'s `Notes/` folder by [`.github/workflows/sync-notes.yml`](.github/workflows/sync-notes.yml):

- Runs **Mon–Fri at 10:00 and 16:00 IST**, plus on-demand via `workflow_dispatch`
- Pulls any new or changed file from the source repo
- Converts anything that isn't already a PDF (images, Office docs, text) into one
- Commits only when content actually changed, authored by **NotBOT**
- Stops running after **2026-07-31** and disables itself

The sync logic lives in [`scripts/sync_notes.py`](scripts/sync_notes.py).

| Topic | File |
|-------|------|
| Introduction to AI/ML | [Intro.pdf](Notes/Intro.pdf) |
| Artificial Intelligence | [Artificial Intelligencr.pdf](Notes/Artificial%20Intelligencr.pdf) |
| Activation Functions | [Activation Functions.pdf](Notes/Activation%20Functions.pdf) |
| Neural Networks | [Neural Networks.pdf](Notes/Neural%20Networks.pdf) |
| Regression | [Regression.pdf](Notes/Regression.pdf) |
| Classification | [Classification.pdf](Notes/Classification.pdf) |
| Decision Trees (Classification) | [Classification-DEcesion_tree.pdf](Notes/Classification-DEcesion_tree.pdf) |
| Decision Tree Regressor | [Decision Tree Regressor.pdf](Notes/Decision%20Tree%20Regressor.pdf) |
| Clustering | [Clustering.pdf](Notes/Clustering.pdf) |
| Encoding | [Encoding.pdf](Notes/Encoding.pdf) |
| Model Evaluation | [Model Evaluation.pdf](Notes/Model%20Evaluation.pdf) |
| Natural Language Processing | [Natural Language Processing.pdf](Notes/Natural%20Language%20Processing.pdf) |
| Artificial Neural Network (ANN) | [ANN.pdf](Notes/ANN.pdf) |
| Convolutional Neural Network (CNN) | [CNN .pdf](Notes/CNN%20.pdf) |
| Recurrent Neural Network (RNN) | [RNN.pdf](Notes/RNN.pdf) |
| CIFAR-10 Dataset | [CIFAR-10 Dataset.pdf](Notes/CIFAR-10%20Dataset.pdf) |

---

### 3. Machine Learning
| Project | Description | Tech | Status |
|---------|-------------|------|--------|
| — | — | — | 🔜 |

---

### 4. Generative AI & Advanced NLP
| Project | Description | Tech | Status |
|---------|-------------|------|--------|
| [Core NLP Fundamentals](NLP/NLP_basics.ipynb) | Foundations of Natural Language Processing | Python, NLTK | ✅ Done |
| [Introduction to BERT](GEN-AI/BERT_Warmup.ipynb) | Hands-on exploration of BERT architecture | Python, Transformers | ✅ Done |
| [BERT-Powered Sentiment Analysis](GEN-AI/BERT_Usecase_Sentiment_Analysis.ipynb) | Text classification and sentiment prediction | Python, Transformers | ✅ Done |
| [Image Gen Diffusion Models](GEN-AI/Diffusion_Model-2.ipynb) | Practical implementation of diffusion models | Python | ✅ Done |
| [Langchain RAG Pipeline](GEN-AI/RAG_Langchain_Example.ipynb) | Retrieval-Augmented Generation using Langchain | Python, Langchain | ✅ Done |
| [Building RAG from Scratch](GEN-AI/RAG_Step_by_Step-2.ipynb) | Custom step-by-step RAG architecture implementation | Python | ✅ Done |
| [Local LLM with Ollama](GEN-AI/ollama.ipynb) | Inferencing local large language models | Python | ✅ Done |
| [Ollama Application Boilerplate](OLLAMA_APP/) | Production-ready standalone UV project scaffold | Python | ✅ Done |

---

### 5. Data Structures & Algorithms
| Topic | Problems | Language | Status |
|-------|----------|----------|--------|
| — | — | — | 🔜 |

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| **Languages** | Python |
| **ML / DL** | TensorFlow, Keras, Scikit-learn, PyTorch, NumPy, Pandas |
| **Visualization** | Matplotlib, Seaborn |
| **Gen AI** | Langchain, Transformers, Ollama, BERT, Diffusion Models |
| **DSA** | *(to be updated)* |

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install -r requirements.txt
```

### Clone & Explore

```bash
git clone https://github.com/vijay-xd/Pep-Learning.git
cd Pep-Learning
jupyter notebook
```

---

## 📈 Progress Tracker

- [x] Neural Networks — Perceptron, ANN, CNN, RNN implementations
- [x] Neural Networks — MNIST digit classification (CNN)
- [x] Course Notes — AI, ML, DL theory (PDFs)
- [ ] Machine Learning — Classification / Regression projects
- [x] Generative AI — LLM / Prompt Engineering projects
- [ ] DSA — Arrays, Linked Lists, Trees, Graphs, DP

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋 Author

**Vijay** — [@vijay-xd](https://github.com/vijay-xd)

---

<p align="center">
  <i>⭐ Star this repo if you find it helpful!</i>
</p>
