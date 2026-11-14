# DSCI 552 — Homework 7

## Environment setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -m ipykernel install --user --name dsci552-hw7 \
  --display-name "Python 3 (DSCI 552 HW7)"
```

All random procedures use `RANDOM_STATE = 42`, so rerunning the complete notebook reproduces the reported results.

The notebook expects the following repository structure:

```text
DSCI552_HW7/
├── data/
│   └── Anuran_Calls_MFCCs/
│       └── Frogs_MFCCs.csv
├── notebook/
│   └── Liau_Olivia_HW7.ipynb
├── README.md
└── requirements.txt
```

Because the dataset is loaded using the relative path `../data/Anuran_Calls_MFCCs/Frogs_MFCCs.csv`, launch Jupyter from the `notebook/` directory:

```bash
cd notebook
jupyter lab
```

Then open `Liau_Olivia_HW7.ipynb`, select the **Python 3 (DSCI 552 HW7)** kernel, and run all cells.

## Data source

[Anuran Calls (MFCCs) — UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/406/anuran+calls+mfccs)