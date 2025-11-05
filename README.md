# Airline Performance Insights ✈️

Python • Pandas • Jupyter Notebook • scikit-learn • Matplotlib / Seaborn

Introduction 📝
---

United Airlines — Flight Analysis & PNR Processing is a data-driven project that analyses flight and PNR data to extract meaningful insights about flight difficulty, baggage patterns, and PNR-level remarks. The project performs cleaning, feature engineering, exploratory data analysis (EDA), and builds models to predict flight difficulty or classify flight/PNR conditions. It's ideal for showcasing data engineering, EDA, and machine-learning skills for airline operations analytics or academic demos.

Features ✨

PNR & Flight Level Aggregation – Combine PNR and flight-level records to create rich, analysis-ready tables.

Data Cleaning & Preprocessing – Handle missing values, normalize categorical fields, parse timestamps, and sanitize text remarks.

Feature Engineering – Create derived features (e.g., connection counts, baggage-level summary, delay buckets, remark sentiment).

Exploratory Data Analysis (EDA) – Visualizations and statistical summaries to spot trends across airports, baggage counts, and flight difficulty.

Flight Difficulty Prediction – Prototype models (classification/regression) to predict flight difficulty score or category using classical ML (e.g., RandomForest, XGBoost).

PNR Remark Analysis – Text processing pipeline to extract actionable signals from PNR remarks (tokenization, TF-IDF, simple NLP features).

Outputs & Reports – Produces CSV outputs and visual plots summarizing model results and operational insights.

Notebook-driven – Main workflow in code.ipynb for easy reproducibility and step-by-step explanation.

Project Structure 📁
United Airlines/
├─ Airports Data.csv                  # Airport metadata (codes, city, country, timezone)
├─ Bag+Level+Data.csv                 # Baggage-level records (per PNR/segment)
├─ Flight Level Data.csv              # Flight-level attributes and operational metrics
├─ PNR Remark Level Data.csv          # Raw PNR remarks (textual)
├─ PNR+Flight+Level+Data.csv          # Joined dataset used for modeling & EDA
├─ code.ipynb                         # Jupyter notebook: full pipeline (EDA → features → models)
├─ flight_difficulty_output.csv       # Final predicted flight difficulty / model outputs
└─ README.md                          # (this file)

Quick Start — Run the Notebook 🚀

Clone or copy the project folder to your machine.

Create a Python environment (recommended venv or conda):

# Using venv
python -m venv venv
source venv/Scripts/activate    # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
# If requirements.txt not present, install essentials:
pip install pandas numpy scikit-learn matplotlib seaborn jupyter nltk


Start Jupyter Notebook:

jupyter notebook code.ipynb


Follow the notebook cells top-to-bottom: data loading → cleaning → feature engineering → EDA → modeling → export.

Key Notebook Sections (what to look for) 📘

0. Setup & imports — required libraries and helper functions.

1. Data Loading — reading CSVs and initial inspection.

2. Cleaning & Normalization — handling missing values, normalizing airport codes, timestamp parsing.

3. Feature Engineering — baggage aggregates, PNR counts, remark-derived flags, delay bins.

4. EDA & Visualizations — distribution plots, airport heatmaps, baggage vs difficulty scatter plots.

5. Modeling — baseline models, cross-validation metrics, feature importance.

6. Predictions & Output — create flight_difficulty_output.csv and summary tables.

7. Conclusions & Next Steps — short recommendations and possible improvements.

Tips & Notes 🛠

CSVs contain spaces/plus signs in filenames (e.g., Bag+Level+Data.csv). Use quotes or escape paths if needed.

For reproducibility, set random seeds in modeling cells (random_state=42).

If notebooks show large outputs (big tables), consider sampling or writing intermediate CSVs to disk.

Use nltk / sklearn for remark text features. Keep preprocessing simple (lowercase, remove punctuation, TF-IDF).

Suggested Improvements / Future Work 🔭

Replace prototype models with production-ready pipelines (sklearn Pipeline + ColumnTransformer).

Add time-series models to capture temporal flight patterns and seasonal effects.

Deploy a lightweight dashboard (Streamlit / Dash) for interactive exploration of EDA and model outputs.

Integrate with real-time flight sources (APIs) for live monitoring and alerts.

Example Commands (useful) 💡
# to regenerate joined dataset from raw CSVs (if notebook includes script)
python scripts/join_datasets.py

# to run a quick modelling script (if provided)
python scripts/run_model.py --config configs/model_config.yaml

Contact / Header

Name: Mayank Raj
Email: ironheart.mayank@gmail.com

College: Delhi Technological University (Formerly DCE)
