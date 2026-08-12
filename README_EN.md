# LB259 - Steel Industry Energy Usage

[Deutsch](README.md) | **English**

LB259 is an IMS school project about analysing and predicting electrical energy usage in a steel industry company. The project uses 2018 measurement data and explores how usage, load type, time-based features and technical metrics relate to each other.

## What problem does it solve?

Industrial energy usage changes depending on time of day, weekday and load situation. This project shows how such usage patterns can be described, prepared and predicted with a simple machine-learning model. For recruiters, the repository is mainly useful because it documents data understanding, privacy thinking, feature preparation, model training and evaluation in notebook form.

## Project Context

- School project in module `LB259`
- Focus: data analysis and simple ML prediction
- Target value: `Usage_kWh`
- Model approach in the notebook: linear regression with `scikit-learn`
- Data file: `Steel_industry_data.csv`
- The notebook content is intentionally kept unchanged so the school project context stays authentic.

## Dataset

The dataset describes electrical energy usage in a steel industry company during 2018. Each row represents a 15-minute interval. It includes:

- electricity usage in kilowatt-hours
- lagging and leading reactive power
- CO2 emissions
- power factors
- time features such as weekday and working-day status
- load type

The goal is to predict `Usage_kWh` and analyse relationships between load type, time and energy usage.

## Repository Structure

```text
.
├── Steel_industry_data.csv
├── data_description.ipynb
├── model.ipynb
├── evaluation.ipynb
└── README.md
```

## Installation

Requirements:

- Python `3.10` or newer
- Git
- Jupyter Notebook or JupyterLab

Windows PowerShell:

```powershell
git clone https://github.com/AleksZyro/LB259.git
cd LB259
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install notebook matplotlib scikit-learn
jupyter notebook
```

macOS or Linux:

```bash
git clone https://github.com/AleksZyro/LB259.git
cd LB259
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install notebook matplotlib scikit-learn
jupyter notebook
```

Open the notebooks in this order:

1. `data_description.ipynb`
2. `model.ipynb`
3. `evaluation.ipynb`

## Privacy

The dataset does not contain personal data. All values describe anonymised energy usage of an industrial process. There is no information about individual people, employees or customers. The data was published in aggregated form and is publicly available. Additional anonymisation is not required for this school project.

## What does it help with?

- Describe datasets from a domain perspective
- Explain privacy for non-personal measurement data
- Analyse CSV data in notebooks
- Prepare simple features for an ML model
- Train and evaluate linear regression
- Interpret results with metrics such as MAE and R2

## Repository Metadata Suggestion

- Description: `School data science project predicting steel industry energy usage with Python notebooks and linear regression.`
- Topics: `python`, `jupyter-notebook`, `data-science`, `machine-learning`, `linear-regression`, `energy-usage`, `steel-industry`, `school-project`
