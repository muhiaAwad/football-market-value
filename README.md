# ⚽ Football Player Market Value Analysis

A data wrangling and analysis project exploring the relationship between football players' attacking performance and their market value.

## 📌 Project Overview

Understanding what drives player valuation is valuable for clubs, scouts, and analysts. This project gathers, wrangles, and analyzes data from two sources to investigate which factors — goals, assists, physical attributes — correlate with a player's market value.

## 📂 Dataset Sources

| Dataset | Source | Method |
|--------|--------|--------|
| Player stats (goals, assists, market value) | [Transfermarkt via Kaggle](https://www.kaggle.com/) | CSV download |
| Physical attributes (height, weight, DOB) | [Sportmonks API](https://www.sportmonks.com/) | REST API (Python) |

**Final dataset:** 26,000+ players after merging and cleaning.

## 🔧 Data Wrangling Pipeline

- **Gathering:** Manual CSV download + programmatic API retrieval
- **Assessing:** Identified missing values, duplicates, and type issues
- **Cleaning:** Merged multiple CSVs using `pandas`, handled nulls, standardized data types

## 📊 Key Questions

1. Do players with more goals have higher market values?
2. Does physical size (height/weight) influence valuation?
3. How do assists compare to goals as a value predictor?

## 🛠️ Technologies Used

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Requests](https://img.shields.io/badge/Requests-API-green?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

- **Python** — Data gathering, wrangling, and analysis
- **Pandas** — Merging, aggregation, and cleaning
- **Requests** — API data retrieval
- **Matplotlib / Seaborn** — Visualization
- **Jupyter Notebook** — Development environment

## 📁 Project Structure

```
football-market-value/
│
├── real_world_data_wrangling.ipynb   # Main notebook (gather → assess → clean → analyze)
├── data/
│   ├── players.csv                   # Transfermarkt player data
│   ├── appearances.csv               # Match appearance stats
│   └── player_valuations.csv         # Historical market values
└── README.md
```

## ⬇️ Download the Data

The `appearances.csv` file exceeds GitHub's file size limit and is not included in this repository. Download it manually:

1. Go to [Football Data from Transfermarkt on Kaggle](https://www.kaggle.com/datasets/davidcariboo/player-scores)
2. Download the dataset
3. Place the following files inside the `data/` folder:
   - `appearances.csv`
   - `players.csv`
   - `player_valuations.csv`

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/muhiaAwad/football-market-value.git
   cd football-market-value
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy requests matplotlib seaborn
   ```

3. Open the notebook:
   ```bash
   jupyter notebook real_world_data_wrangling.ipynb
   ```

> **Note:** To use the Sportmonks API, you'll need your own API token at [sportmonks.com](https://www.sportmonks.com/).

## 📝 Part of

**Udacity Data Analyst Nanodegree** — Advanced Data Wrangling Project
