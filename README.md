# LB259 - Energieverbrauch in der Stahlindustrie

**Deutsch** | [English](README_EN.md)

LB259 ist ein IMS-Schulprojekt zur Analyse und Vorhersage des elektrischen Energieverbrauchs eines Stahlindustrieunternehmens. Die Arbeit nutzt Messwerte aus dem Jahr 2018 und untersucht, wie Verbrauch, Lasttyp, Zeitmerkmale und weitere technische Kennzahlen zusammenhängen.

## Welches Problem löst das Projekt?

Industriebetriebe verbrauchen je nach Tageszeit, Wochentag und Lastsituation unterschiedlich viel Energie. Das Projekt zeigt anhand eines Datensatzes, wie solche Verbrauchsmuster beschrieben, vorbereitet und mit einem einfachen Machine-Learning-Modell vorhergesagt werden können. Für Recruiter ist das Repository vor allem interessant, weil es Datenverständnis, Datenschutzüberlegung, Feature-Aufbereitung, Modelltraining und Evaluation in Notebook-Form dokumentiert.

## Projektkontext

- Schulprojekt im Modul `LB259`
- Fokus: Datenanalyse und einfache ML-Vorhersage
- Zielwert: `Usage_kWh`
- Modellansatz im Notebook: lineare Regression mit `scikit-learn`
- Datenquelle: `Steel_industry_data.csv`
- Die fachlichen Notebook-Inhalte bleiben bewusst unverändert, damit der Schulprojekt-Charakter erhalten bleibt.

## Datensatz

Der verwendete Datensatz beschreibt den elektrischen Energieverbrauch eines Stahlindustrieunternehmens über das Jahr 2018. Jede Zeile enthält ein 15-Minuten-Zeitintervall. Enthalten sind unter anderem:

- Stromverbrauch in Kilowattstunden
- Blindleistung
- CO2-Emissionen
- Leistungsfaktoren
- Zeitmerkmale wie Wochentag und Arbeitstagstatus
- Lasttyp

Ziel des Projekts ist es, auf Basis dieser Merkmale den Energieverbrauch (`Usage_kWh`) vorherzusagen und Zusammenhänge zwischen Lasttyp, Zeit und Verbrauch zu analysieren.

## Repository-Struktur

```text
.
├── Steel_industry_data.csv
├── data_description.ipynb
├── model.ipynb
├── evaluation.ipynb
└── README.md
```

## Installation

Voraussetzungen:

- Python `3.10` oder neuer
- Git
- Jupyter Notebook oder JupyterLab

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

macOS oder Linux:

```bash
git clone https://github.com/AleksZyro/LB259.git
cd LB259
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install notebook matplotlib scikit-learn
jupyter notebook
```

Danach die Notebooks in dieser Reihenfolge öffnen:

1. `data_description.ipynb`
2. `model.ipynb`
3. `evaluation.ipynb`

## Datenschutz

Der Datensatz enthält keine personenbezogenen Daten. Alle Messwerte beziehen sich auf den anonymisierten Energieverbrauch eines industriellen Prozesses. Es sind keine Informationen zu einzelnen Personen, Mitarbeitenden oder Kunden enthalten. Die Daten wurden aggregiert veröffentlicht und sind frei zugänglich. Zusätzliche Anonymisierung ist für dieses Schulprojekt nicht nötig.

## Wobei hilft das Projekt?

- Datensätze fachlich beschreiben
- Datenschutz bei nicht-personenbezogenen Messdaten erklären
- CSV-Daten in Notebooks auswerten
- einfache Features für ein ML-Modell vorbereiten
- lineare Regression trainieren und evaluieren
- Resultate mit Metriken wie MAE und R2 einordnen

## Repository-Metadaten Vorschlag

- Description: `School data science project predicting steel industry energy usage with Python notebooks and linear regression.`
- Topics: `python`, `jupyter-notebook`, `data-science`, `machine-learning`, `linear-regression`, `energy-usage`, `steel-industry`, `school-project`
