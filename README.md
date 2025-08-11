# NLP Workshop

This repository hosts **four** hands-on workshops designed to introduce practical techniques in Natural Language Processing (NLP).

---

## 📋 Table of Contents

- [Overview](#user-content--overview)  
- [Prerequisites](#user-content-️-prerequisites)  
- [Installation](#user-content--installation)  
- [Usage](#user-content-️-usage)  
- [Workshop 1 - Web Crawling](#user-content--workshop-1-web-crawling)  
- [Workshop 2 - NLP Frameworks](#user-content--workshop-2-nlp-frameworks)  
- [Workshop 3 - PyTorch](#user-content--workshop-3-pytorch)
- [Workshop 4 – Hugging Face](#user-content--workshop-4-hugging-face)
- [Directory Structure](#user-content--directory-structure)  
- [License](#user-content--license)

---

## 📝 Overview

| # | Workshop       | Focus                          | Highlights                                                           |
|---|----------------|--------------------------------|----------------------------------------------------------------------|
| 1 | Web Crawling   | Collecting text from the web   | `requests`, BeautifulSoup, Selenium, pagination, dynamic content     |
| 2 | NLP Frameworks | Classic & Persian NLP toolkits | NLTK, spaCy, Hazm, Parsivar, Parsi.io, quick Transformers tour       |
| 3 | PyTorch        | Deep learning essentials       | Tensors, device placement (CPU/CUDA/MPS), autograd, simple NN        |
| 4 | Hugging Face   | Modern NLP workflows           | Hub, `datasets`, `transformers` pipelines, Trainer/PEFT, push to Hub |

Each notebook includes examples, code snippets, and exercises to reinforce learning.

---

## ⚙️ Prerequisites

- **Python 3.8 or higher**
- **pip** (Python package installer)
- **Jupyter Notebook / JupyterLab**  
- (For Workshop 1) a browser driver such as **ChromeDriver**  
- (For Workshop 3) **PyTorch 2.x** with optional CUDA/MPS support
- (For Workshop 4) A free [Hugging Face](https://huggingface.co/) account

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
    - `Workshop 1 - Web Crawling`
    - `Workshop 2 - NLP Frameworks`
    - `Workshop 3 - PyTorch`

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

## 🛠 Workshop 3: PyTorch

Notebook:

- `pytorch.ipynb`

Topics covered:

- Tensors vs. NumPy arrays & device placement (CPU / CUDA / MPS)
- Reproducibility with `torch.manual_seed`
- Automatic differentiation (**autograd**)
- Building a simple feed-forward network for image classification

---

## 🛠 Workshop 4: Hugging Face

Notebook:

- `hugging face.ipynb`

Topics covered:

- Exploring the Hugging Face Hub, finding a model and a dataset, and also inspecting model cards and dataset splits/tags.
- Running zero-shot and few-shot inference with `transformers` pipelines (e.g., text classification or NER).
- Loading a public dataset with `datasets.load_dataset`, then split, shuffle, and map tokenization with `AutoTokenizer`.
- Fine-tuning a pretrained model using the `Trainer` API (define `TrainingArguments`, `compute_metrics`, and evaluation loop).
- (Optional) Apply parameter-efficient fine-tuning (LoRA/PEFT) to reduce VRAM and speed up training.
- Track metrics with `evaluate` (e.g., accuracy/F1) and save the best checkpoint.
- (Optional) Publish a simple demo (Gradio/Spaces) so others can try your model from the browser.

---

## 📂 Directory Structure

```
nlp-workshop/
├── Workshop 1 - Web Crawling/
│   ├── Workshop1 (Crawling-beautifulsoup-selenium).ipynb
│   └── new_Workshop_(Crawling_beautifulsoup_selenium).ipynb
├── Workshop 2 - NLP Frameworks/
│   ├── 1) nltk.ipynb
│   ├── 2) spacy.ipynb
│   ├── 3) hazm.ipynb
│   ├── 4) parsivar.ipynb
│   ├── 5) parsi.io.ipynb
│   └── 6) hugging face.ipynb
├── Workshop 3 - PyTorch/
│   └── pytorch.ipynb
├── Workshop 4 - Hugging Face/
│   └── hugging face.ipynb
├── requirements.txt
└── README.md
```

---

## 📄 License

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.
