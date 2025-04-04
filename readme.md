# SIKT Model Codebase

This repository provides the implementation of the **SIKT** (Side Information Knowledge Tracing) model for knowledge tracing tasks. It includes code for model training, data preprocessing, and t-SNE visualization.

---

## 📁 Project Structure

```
SIKT/
├── model/
│   ├── checkpoints/         # Saved model checkpoints
│   ├── log/                 # Training logs (includes logs from our paper)
│   └── SIKT Model.ipynb     # Main notebook for continual sequence training and joint training
│
├── DataProcess/
│   ├── raw_data/            # Raw data for three datasets: ASSIST2009NSB (A09), ASSIST2012 (A12), EdNet (EN)
│   ├── train_data/          # Preprocessed training data
│   ├── test_data/           # Preprocessed testing data
│   ├── Data Process.ipynb   # Data preprocessing notebook (required to reproduce paper results)
│   └── t-SNE.ipynb          # t-SNE visualization code
│
└── requirements.txt         # Dependencies file (for conda environment setup)
```

---

## ⚙️ Setup

**Platform:** Linux-64  
**RAM Required:** ≥ 120 GB  
**Python Version:** 3.8

### Environment Installation

To create a virtual environment using the `requirements.txt` file, run:

```bash
conda create --name sikt_env --file requirements.txt
conda activate sikt_env
```

Alternatively, you can install dependencies manually using:

```bash
pip install -r requirements.txt
```

We recommend using **Jupyter Notebook** to run the code. You may also convert the notebooks to `.py` scripts if preferred.

---

## 🚀 Running the SIKT Model

To quickly run and observe the SIKT model training process:

1. Open `model/SIKT Model.ipynb`.
2. Run all cells.

⚠️ Note: Due to the large size of the raw datasets, the default notebook only uses the **first 50,000 records** from each dataset for demonstration purposes.

---

## 🛠 Reproducing Paper Results

To fully reproduce the results reported in our paper:

1. Open `DataProcess/Data Process.ipynb`.
2. Run all cells to preprocess the raw data and generate the required training/testing files.

💡 **Tip:** This step is computationally intensive and memory-heavy. Make sure your machine has sufficient resources.

3. After preprocessing is complete, re-run `model/SIKT Model.ipynb` to begin training with the full datasets.

---

## 📊 t-SNE Visualization

After completing the data preprocessing:

1. Open `DataProcess/t-SNE.ipynb`.
2. Run the notebook to visualize the feature distributions of the three datasets using t-SNE.

---

## 📬 Contact

For any questions or feedback, please feel free to contact us or open an issue.
