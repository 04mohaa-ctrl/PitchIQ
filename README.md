# ⚽ PitchIQ

A football analytics and scouting platform built with Python and machine learning.

The project uses event data from Wyscout to analyse matches and players, create advanced football metrics, and build machine-learning models for football analysis.

## 🎯 Project Goals

The goal is to build an interactive football analytics platform capable of:

- Shot maps
- Passing maps
- Player heatmaps
- Expected Goals (xG)
- Player comparison
- Player profiling and clustering
- Match outcome prediction
- Interactive scouting dashboard

## 🤖 Current Progress

### xG Model v1

The first Expected Goals model has been implemented using logistic regression.

Current features:

- Distance to goal
- Shot angle
- Body part

Dataset:

- 380 matches
- 8,451 shots

Current model performance:

- ROC-AUC: ~0.754
- Brier Score: ~0.086
- Baseline Brier Score: ~0.097

The model is also used to calculate player-level statistics including:

- Shots
- Goals
- xG
- Goals minus xG

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- scikit-learn
- Matplotlib
- mplsoccer
- socceraction
- Jupyter
- PostgreSQL (planned)
- Streamlit / React (planned)

## 📁 Project Structure

```text
football-scout-ai/
├── data/
├── notebooks/
│   ├── exploration.ipynb
│   └── wyscout_exploration.ipynb
├── src/
│   ├── data_loader.py
│   └── visualizations.py
├── README.md
├── requirements.txt
└── .gitignore