# Ibovespa Forecasting System

This project demonstrates the development of a **machine learning system for forecasting the daily direction of the Ibovespa index**. The methodology combines:

- Data analysis and feature engineering
- AI-driven hyperparameter optimization (Optuna)
- Rigorous out-of-sample and holdout validation

The final model achieved **75.76% accuracy** on unseen data while operating selectively in high-conviction scenarios, demonstrating not only predictive ability but also risk management.

## Key Features

- Feature engineering based on historical data (1990-2024)
- Model optimization using Optuna
- TimeSeriesSplit and holdout validation for robust evaluation
- Risk-aware selective trading strategy simulation

## Project Structure
```
ibovespa-forecasting-system/
│
├── data/
│   ├── processed/
│   │   └── modelo_final_holdout_lgbm.pkl
│   └── raw/
│       └── ibov.csv
│
└── notebooks/
|    └── 01_data_analysis_and_trainnig_model.ipynb
│
├── README.md               # Project overview and documentation
└── requirements.txt        # Python dependencies
```


## Installation

```bash
git clone https://github.com/GabrielHenriqueCA/ibovespa-forecasting-system.git
cd ibovespa-forecasting-system
pip install -r requirements.txt
