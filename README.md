# COMP3610-A2

Machine learning model training, tuning, evaluation, and interpretation for NYC Yellow Taxi tips.

This repository contains the submission for **COMP 3610 Assignment 2**.

## Assignment Scope

The notebook implements:
- Part 1: Data preprocessing and feature engineering
- Part 2: Baseline models, hyperparameter tuning, and a PyTorch neural network
- Part 3: Test-set evaluation, interpretation, and written analysis

Prediction tasks:
- Regression: predict `tip_amount`
- Classification: predict `high_tip` where `tip_amount > 20% of fare_amount`

## Repository Structure

- `assignment2.ipynb`: main notebook submission
- `requirements.txt`: pinned Python dependencies
- `.gitignore`: ignore rules for environments, data files, and artifacts
- `README.md`: project overview and setup instructions

## Requirements

- Python 3.10+ (tested with Python 3.12)
- `pip`

## Setup Instructions

### Windows (PowerShell)

```powershell
python -m venv .venv
.venv\Scripts\Activate
pip install --upgrade pip
pip install -r requirements.txt
```

### macOS/Linux (bash/zsh)

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## How To Run

1. Start Jupyter:

```bash
jupyter notebook
```

2. Open `assignment2.ipynb`.
3. Run all cells from top to bottom.

Notes:
- The notebook downloads raw NYC taxi data automatically if not present.
- Hyperparameter tuning is compute-intensive and may take significant time on CPU.

## Reproducibility

- Random operations use a fixed seed (`RANDOM_STATE = 42`).
- Hyperparameter tuning uses `RandomizedSearchCV` with reproducible settings.

## AI Disclosure

An `AI Tools Used` section is included at the end of `assignment2.ipynb`, as required by the assignment instructions.