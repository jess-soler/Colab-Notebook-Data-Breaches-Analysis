# Data Breaches Analysis Notebook

This repository contains a **Google Colab notebook** for analyzing the dataset [Data Breaches: A Comprehensive List](https://www.kaggle.com/datasets/thedevastator/data-breaches-a-comprehensive-list) from Kaggle. The notebook automatically downloads the dataset using **KaggleHub** and loads it into **Pandas** for analysis.

---

## Features

- Automatically installs required dependencies (`kagglehub`, `pandas`).
- Handles Kaggle API authentication via `kaggle.json`.
- Downloads the latest version of the dataset directly from Kaggle.
- Automatically detects and loads the CSV file into a Pandas DataFrame.
- Ready for analysis without manual file management.

---

## Getting Started

### 1. Open the Notebook in Colab
Click [here](https://colab.research.google.com/github/YOUR_USERNAME/YOUR_REPO/blob/main/YOUR_NOTEBOOK.ipynb) to open the notebook in Google Colab.

### 2. Get Your Kaggle API Key
1. Go to [Kaggle Account Settings](https://www.kaggle.com/settings/account).
2. Scroll to **API** and click **Create New API Token**.
3. Download `kaggle.json` (your API key).

### 3. Run the Notebook
1. Upload `kaggle.json` when prompted.
2. The notebook will automatically:
   - Install dependencies.
   - Authenticate with Kaggle.
   - Download the dataset.
   - Load the first CSV file into a Pandas DataFrame.
3. After the first cell, your dataset is ready for analysis.

---

## Notes

- **Do not commit your `kaggle.json` to GitHub** — it contains your private API key.
- This notebook works for anyone with a Kaggle account; each user must provide their own `kaggle.json`.
- The notebook is designed to work even if the CSV filename changes in the dataset.

---

## Example Usage

```python
# Inspect dataset
df.head()

# Basic statistics
df.describe()

# Filter by year
df_2010s = df[df['Year'] > 2010]

---

## Screenshot

Here’s a preview of the notebook in Colab:

<img src="images/screenshot.png" width="700">

---


