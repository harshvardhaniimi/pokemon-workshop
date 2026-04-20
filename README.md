# Can a Machine Tell Pokémon Types Apart?

**SBA Workshop organized by MODA and BAA · American University of Sharjah**

A gentle introduction to machine learning. We build small classifiers that look at a Pokémon's image and guess whether it is **Fire**, **Water**, or **Grass** type — using only the colours in the image.

No prior coding or machine-learning background required.

---

## Getting started (the easy way)

Click the button below. The notebook opens in your browser via **Google Colab**, downloads the data automatically, and runs end-to-end without any local setup.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/harshvardhaniimi/pokemon-workshop/blob/main/Pokemon_Workshop.ipynb)

Run each grey cell from top to bottom by clicking inside it and pressing **Shift + Enter**.

---

## Getting started (on your laptop)

If you prefer to run things locally, first clone the repo and install the packages:

```bash
git clone https://github.com/harshvardhaniimi/pokemon-workshop.git
cd pokemon-workshop
pip install numpy pandas matplotlib scikit-learn pillow jupyter
```

Then open the notebook in **either** of these two ways.

### Option A — Jupyter Notebook (browser)

```bash
jupyter notebook Pokemon_Workshop.ipynb
```

A browser tab will open with the notebook. Click any grey cell and press **Shift + Enter** to run it.

### Option B — VSCode (recommended if you already use it)

1. Install [VSCode](https://code.visualstudio.com/) if you don't have it.
2. Inside VSCode, open the **Extensions** tab (`Ctrl/Cmd + Shift + X`) and install **Python** and **Jupyter** (both from Microsoft).
3. Open the workshop folder: `File → Open Folder…` → pick `pokemon-workshop`. (Or from the terminal: `code pokemon-workshop`.)
4. In the file tree on the left, click `Pokemon_Workshop.ipynb`.
5. The first time you run a cell, VSCode will ask you to pick a Python kernel — choose any Python install that has the packages from above.
6. Run cells one at a time with the ▶ button next to each cell, or press **Shift + Enter**. Or hit **"Run All"** at the top to run the whole notebook at once.

The notebook itself downloads the data the first time you run it, so there is nothing else to set up.

---

## What's in this repo

```
pokemon-workshop/
├── Pokemon_Workshop.ipynb     ← The main notebook (open this!)
├── pokemon_data.zip           ← 721 Pokémon images + type labels
├── slides/
│   ├── Pokemon_Workshop_Slides.pdf   ← Workshop slides
│   ├── Pokemon_Workshop_Slides.tex   ← LaTeX source
│   └── figures/                       ← Slide figures
└── README.md
```

---

## What you will learn

The workshop walks through:

1. **What is machine learning?** Programming with data instead of explicit rules.
2. **How a computer sees an image** — as a grid of Red/Green/Blue pixel values.
3. **Features** — turning each image into just three numbers (the average R, G, B).
4. **Two model families** — Random Forests and Logistic Regression.
5. **Evaluation** — accuracy and confusion matrices.
6. **Hyperparameter tuning** — using `GridSearchCV` with cross-validation.
7. **Two big lessons** that contradict the usual hype:
   - Tuning is useful but not magic.
   - Picking the right model family often matters more than tuning.

There is also an **optional bonus section** at the end of the notebook on **PCA** (Principal Component Analysis) — what it is, when to use it, and a third lesson about why good features can beat fancy techniques. We won't cover this live; try it at home.

---

## Data

The dataset contains 721 Pokémon images (one per Pokémon, generations 1–7) with type labels in `pokemon.csv`. We filter to the three most visually distinctive types — **Fire** (53), **Water** (114), and **Grass** (78) — for a total of 245 Pokémon.

Original source: Vishal Subbiah, *Pokémon Images and Types* (Kaggle).

---

## Workshop materials

- **Slides** — [`slides/Pokemon_Workshop_Slides.pdf`](slides/Pokemon_Workshop_Slides.pdf) walks through the concepts before we open the notebook.
- **Notebook** — [`Pokemon_Workshop.ipynb`](Pokemon_Workshop.ipynb) is the hands-on portion of the workshop.

---

## Contact

Workshop by Dr. Harshvardhan · Organised by MODA and BAA · School of Business Administration · American University of Sharjah
