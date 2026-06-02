# ⚽ FIFA 2026 Winner Prediction using XGBoost and ELO Ratings

## Overview

This project predicts FIFA World Cup 2026 match outcomes and potential tournament winners using Machine Learning, ELO ratings, team form statistics, head-to-head records, and historical international football match data.

The system collects historical match results, engineers predictive features, trains an XGBoost classifier, and generates predictions for FIFA World Cup 2026 fixtures.

---

## 🚀 Features

- Historical international football match analysis
- Dynamic ELO rating calculation
- Team form analysis
- Goal scoring and conceding statistics
- Head-to-head performance tracking
- Tournament importance weighting
- XGBoost-based match outcome prediction
- FIFA World Cup 2026 fixture simulation
- Probability-based match forecasts

---

## 📂 Project Structure

```text
FIFA-2026-Winner-Prediction/
│
├── data/
│   ├── match_results.csv
│   ├── elo_ratings.csv
│   ├── current_elo.csv
│   ├── 2026_teams.csv
│   ├── features_train.csv
│   ├── features_test.csv
│   ├── features_2026.csv
│   └── 2026_predictions.csv
│
├── notebooks/
│   ├── collect_data.ipynb
│   ├── feature_engineering.ipynb
│   └── model_training.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📊 Dataset

### Historical Match Results

The dataset contains:

- International football matches
- Match dates
- Home and away teams
- Scores
- Tournament information
- Neutral venue information

### ELO Ratings

ELO ratings are used to estimate team strength over time and are updated after each match based on actual and expected results.

---

## 🔧 Feature Engineering

The model uses the following features:

### ELO Features

- Home ELO
- Away ELO
- ELO Difference
- ELO Win Probability

### Team Form Features

- Home Team Recent Form
- Away Team Recent Form
- Form Difference

### Goal Statistics

- Average Goals Scored
- Average Goals Conceded
- Expected Goal Difference (XGD)

### Head-to-Head Features

- Home Team Win Rate
- Historical Draw Rate

### Match Context Features

- Tournament Weight
- Neutral Venue Indicator
- World Cup Indicator

---

## 🤖 Machine Learning Model

### Algorithm

**XGBoost Classifier**

### Prediction Classes

| Class | Meaning |
|---------|----------|
| 0 | Away Win |
| 1 | Draw |
| 2 | Home Win |

### Model Configuration

- 200 Estimators
- Maximum Tree Depth: 6
- Learning Rate: 0.1
- Subsample: 0.8
- Feature Subsample: 0.8

---

## 🔄 Workflow

```text
Historical Match Data
          ↓
ELO Calculation
          ↓
Feature Engineering
          ↓
Train/Test Split
          ↓
XGBoost Training
          ↓
Model Evaluation
          ↓
2026 Fixture Prediction
          ↓
World Cup Simulation
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/FIFA-2026-Winner-Prediction.git
cd FIFA-2026-Winner-Prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

### Step 1: Data Collection

Run:

```bash
collect_data.ipynb
```

Generates:

- match_results.csv
- elo_ratings.csv
- current_elo.csv
- 2026_teams.csv

### Step 2: Feature Engineering

Run:

```bash
feature_engineering.ipynb
```

Generates:

- features_train.csv
- features_test.csv
- features_2026.csv

### Step 3: Model Training

Run:

```bash
model_training.ipynb
```

Outputs:

- Model Accuracy
- Classification Report
- Feature Importance
- 2026 Match Predictions

---

## 📈 Example Prediction

```text
Argentina vs Mexico

Home Win Probability : 68.4%
Draw Probability     : 18.2%
Away Win Probability : 13.4%

Predicted Result: Argentina Win
```

---

## 🔮 Future Improvements

- Streamlit Web Application
- Interactive Tournament Simulator
- Knockout Stage Simulation
- Monte Carlo Tournament Forecasting
- Real-Time FIFA Ranking Updates
- REST API Integration
- Mobile Application

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- Matplotlib
- Jupyter Notebook

---

## 👨‍💻 Author

**Protyay Saha**

---

## 📜 License

This project is licensed under the MIT License.
