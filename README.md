# NLP Workshop

This repository hosts **three** hands-on workshops designed to introduce practical techniques in Natural Language Processing (NLP).  
Each workshop is provided as a Jupyter notebook:

1. **Web Crawling** – collecting textual data from the Web.  
2. **NLP Frameworks** – getting to know popular libraries for English and Persian.  
3. **PyTorch** – the essentials of deep-learning with PyTorch for NLP.

---

## 📋 Table of Contents

- [Overview](#user-content--overview)  
- [Prerequisites](#user-content--prerequisites)  
- [Installation](#user-content--installation)  
- [Usage](#user-content--usage)  
- [Workshop 1 – Web Crawling](#user-content--workshop-1-web-crawling)  
- [Workshop 2 – NLP Frameworks](#user-content--workshop-2-nlp-frameworks)  
- [Workshop 3 – PyTorch](#user-content--workshop-3-pytorch)  
- [Directory Structure](#user-content--directory-structure)  
- [License](#user-content--license)

---

## 📝 Overview

| Workshop | Focus | Highlights |
| -------- | ----- | ---------- |
| **1** | Web Crawling | HTTP requests, BeautifulSoup, Selenium, pagination, dynamic content |
| **2** | NLP Frameworks | NLTK, spaCy, Hazm, Parsivar, Parsi.io, 🤗 Transformers |
| **3** | PyTorch | Tensors, GPU/CPU device management, automatic differentiation, basic neural-net layers, mini image-classification exercise |

Each notebook includes examples, code snippets, and exercises to reinforce learning.

---

## ⚙️ Prerequisites

- **Python 3.8 or higher**
- **pip** (Python package installer)
- **Jupyter Notebook / JupyterLab**  
- (For Workshop 1) a browser driver such as **ChromeDriver**  
- (For Workshop 3) **PyTorch 2.x** with optional CUDA/MPS support

---

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/language-ml/nlp-workshop.git
   cd nlp-workshop
   ```

2. **Create a virtual environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **(Optional) Download language models**
   ```bash
   # NLTK
   python -c "import nltk; nltk.download('punkt_tab','averaged_perceptron_tagger')"

   # spaCy (English model)
   python -m spacy download en_core_web_sm
   python -m spacy download en_core_web_md
   ```

   4. **(optional) install PyTorch**
   ```bash
   pip install torch torchvision torchaudio
   ```

---

## ▶️ Usage

1. **Activate the environment** (if not already active):
   ```bash
   source venv/bin/activate
   ```

2. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

3. **Open the desired notebook** under the folders:
    - `Workshop 1 – Web Crawling`
    - `Workshop 2 – NLP Frameworks`
    - `Workshop 3 – PyTorch`

4. **Follow the instructions** and run cells interactively.

---

## 💡 Workshop 1: Web Crawling

Notebook list:

- `Workshop1 (Crawling-beautifulsoup-selenium).ipynb`
- `new_Workshop_(Crawling_beautifulsoup_selenium).ipynb`

Topics covered:

- HTTP requests with `requests`
- Parsing HTML with **BeautifulSoup**
- Automating browser actions with **Selenium**
- Handling pagination and dynamic content

---

## 💼 Workshop 2: NLP Frameworks

Notebook sequence:

1. `1) nltk.ipynb`
2. `2) spacy.ipynb`
3. `3) hazm.ipynb`
4. `4) parsivar.ipynb`
5. `5) parsi.io.ipynb`
6. `6) hugging face.ipynb`

Topics covered:

- Tokenization, POS-tagging & parsing (English & Persian)
- Pre-built pipelines in **NLTK**, **spaCy**, **Hazm**, **Parsivar**
- Using **Parsi.io** APIs for Persian NLP
- Quick tour of 🤗 **Transformers** for text classification and generation

---

## 🛠️ Workshop 3: PyTorch

Notebook:

- `pytorch.ipynb`

Topics covered:

- Tensors vs. NumPy arrays & device placement (CPU / CUDA / MPS)
- Reproducibility with `torch.manual_seed`
- Automatic differentiation (**autograd**)
- Building a simple feed-forward network for image classification

---

## 📂 Directory Structure

```
nlp-workshop/
├── Workshop 1 – Web Crawling/
│   ├── Workshop1 (Crawling-beautifulsoup-selenium).ipynb
│   └── new_Workshop_(Crawling_beautifulsoup_selenium).ipynb
├── Workshop 2 – NLP Frameworks/
│   ├── 1) nltk.ipynb
│   ├── 2) spacy.ipynb
│   ├── 3) hazm.ipynb
│   ├── 4) parsivar.ipynb
│   ├── 5) parsi.io.ipynb
│   └── 6) hugging face.ipynb
├── Workshop 3 – PyTorch/
│   └── pytorch.ipynb
├── requirements.txt
└── README.md
```

---

## 📄 License

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.
