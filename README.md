
# Primetrade.ai: Trader Performance vs Market Sentiment

This repository contains the Data Analyst Intern project (Round-0 Assignment) for Primetrade.ai. The study analyzes historical Hyperliquid trader transaction data against Bitcoin's daily Fear & Greed index to uncover structural behavioral patterns, regime-based performance shifts, and archetypal trader clustering.

## 📂 Repository Structure

The project has been organized into modular directories for better data governance:

```text
├── data/
│   ├── historical_data.csv            # Hyperliquid execution logs
│   └── fear_greed_index.csv           # Daily Bitcoin sentiment classifications
├── notebook/
│   └── trader_sentiment_analysis.ipynb # Main Jupyter Notebook for EDA & Clustering
├── output/
│   ├── charts/                        # Generated visual insights & plots
│   └── tables/                        # Statistical summaries and cluster metrics
├── Data Science Intern project.pdf     # assignment
├── trader_sentiment_analysis_summary.md # Quick-read executive summary
└── README.md                          # Repository documentation (this file)

```

> **Note on Notebook Pathing:** The notebook inside `notebook/` uses relative paths (`../data/filename.csv`) to automatically reach the datasets without requiring you to move files around.

## 🚀 How to Run

This project is designed to be completely plug-and-play. You can easily run it locally or via the cloud.

### Option 1: Run Locally (Jupyter Notebook)

1. **Clone or extract** the repository files keeping the directory structure intact.
2. Open **Jupyter Notebook** or **Jupyter Lab**, navigate to the `notebook/` directory, and open `trader_sentiment_analysis.ipynb`.
3. Click **"Run All"** to execute the pipeline. The notebook will automatically pull data from the `data/` folder and save fresh assets into the `output/` folder.

### Option 2: Run in the Cloud (Google Colab)

1. Open [Google Colab](https://colab.research.google.com/).
2. Click **File > Upload notebook** and select the `trader_sentiment_analysis.ipynb` file from the `notebook/` folder.
3. On the left sidebar, click the **Folder icon** (Files). Create a new folder named `data` and upload both `.csv` files inside it so the notebook's relative paths (`../data/...`) resolve correctly.
4. Click **Runtime > Run all**.

## 📦 Dependencies

The pipeline utilizes standard Python data science libraries. If running locally, ensure you have the following installed:
`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`