# NLP Workshop

This repository contains two hands-on workshops designed to introduce practical techniques in Natural Language
Processing (NLP). Each workshop is provided as a Jupyter notebook, covering web crawling and core NLP frameworks (
including several Persian‑language tools).

---

## 📋 Table of Contents

- [Overview](https://github.com/language-ml/nlp-workshop?tab=readme-ov-filehttps://github.com/language-ml/nlp-workshop?tab=readme-ov-file#overview)
- [Prerequisites](https://github.com/language-ml/nlp-workshop?tab=readme-ov-file#prerequisites)
- [Installation](https://github.com/language-ml/nlp-workshop?tab=readme-ov-file#installation)
- [Usage](https://github.com/language-ml/nlp-workshop?tab=readme-ov-file#usage)
- [Workshop 1: Web Crawling](https://github.com/language-ml/nlp-workshop?tab=readme-ov-file#workshop-1-web-crawling)
- [Workshop 2: NLP Frameworks](https://github.com/language-ml/nlp-workshop?tab=readme-ov-file#workshop-2-nlp-frameworks)
- [Directory Structure](https://github.com/language-ml/nlp-workshop?tab=readme-ov-file#directory-structure)
- [Contributing](https://github.com/language-ml/nlp-workshop?tab=readme-ov-file#contributing)
- [License](https://github.com/language-ml/nlp-workshop?tab=readme-ov-file#license)

---

## 📝 Overview

- **Workshop 1:** Learn how to fetch and parse web pages programmatically using BeautifulSoup and Selenium.
- **Workshop 2:** Explore popular NLP libraries and frameworks:
    - **NLTK** (general NLP)
    - **spaCy** (industrial‑strength NLP)
    - **Hazm**, **Parsivar**, **Parsi.io** (Persian‑language processing)
    - **Hugging Face Transformers** (state‑of‑the‑art models)

Each notebook includes examples, code snippets, and exercises to reinforce learning.

---

## ⚙️ Prerequisites

- **Python 3.8 or higher**
- **pip** (Python package installer)
- **Web browser drivers** (for Selenium; e.g., ChromeDriver)

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

4. **Follow the instructions** and run cells interactively.

---

## 💡 Workshop 1: Web Crawling

Notebooks:

- `Workshop1 (Crawling-beautifulsoup-selenium).ipynb`
- `new_Workshop_(Crawling_beautifulsoup_selenium).ipynb`

Topics covered:

- HTTP requests with `requests`
- Parsing HTML with **BeautifulSoup**
- Automating browser actions with **Selenium**
- Handling pagination and dynamic content

---

## 💼 Workshop 2: NLP Frameworks

Notebooks:

1. **NLTK**: `1) nltk.ipynb`
2. **spaCy**: `2) spacy.ipynb`
3. **Hazm** (Persian): `3) hazm.ipynb`
4. **Parsivar** (Persian): `4) parsivar.ipynb`
5. **Parsi.io** (Persian): `5) parsi.io.ipynb`
6. **Hugging Face Transformers**: `6) hugging face.ipynb`

Each notebook introduces the library’s core APIs, demonstrates text processing pipelines, and includes practice
exercises.

Additional resources are available in the `resources/` folder (e.g., sample text files, helper scripts).

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
│   ├── 6) hugging face.ipynb
│   └── resources/
├── requirements.txt
└── README.md
```

---

## 🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request with:

- Bug fixes
- Layout or documentation improvements
- New workshop modules or exercises

Before submitting, ensure:

- Code runs without errors
- Notebooks are clean (clear outputs)

---

## 📄 License

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.
