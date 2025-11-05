# Airline Performance Insights ✈️

Python • Pandas • Jupyter Notebook • scikit-learn • Matplotlib / Seaborn

Introduction 📝
---

United Airlines — Flight Analysis & PNR Processing is a data-driven project that analyses flight and PNR data to extract meaningful insights about flight difficulty, baggage patterns, and PNR-level remarks. The project performs cleaning, feature engineering, exploratory data analysis (EDA), and builds models to predict flight difficulty or classify flight/PNR conditions. It's ideal for showcasing data engineering, EDA, and machine-learning skills for airline operations analytics or academic demos.

Features ✨
---

* PNR & Flight Level Aggregation – Combine PNR and flight-level records to create rich, analysis-ready tables.

* Data Cleaning & Preprocessing – Handle missing values, normalize categorical fields, parse timestamps, and sanitize text remarks.

* Feature Engineering – Create derived features (e.g., connection counts, baggage-level summary, delay buckets, remark sentiment).

* Exploratory Data Analysis (EDA) – Visualizations and statistical summaries to spot trends across airports, baggage counts, and flight difficulty.

* Flight Difficulty Prediction – Prototype models (classification/regression) to predict flight difficulty score or category using classical ML (e.g., RandomForest, XGBoost).

* PNR Remark Analysis – Text processing pipeline to extract actionable signals from PNR remarks (tokenization, TF-IDF, simple NLP features).

* Outputs & Reports – Produces CSV outputs and visual plots summarizing model results and operational insights.

* Notebook-driven – Main workflow in code.ipynb for easy reproducibility and step-by-step explanation.

Project Structure 📁
---

Airlines/
├─ Airports Data.csv                  # Airport metadata (codes, city, country, timezone)
├─ Bag+Level+Data.csv                 # Baggage-level records (per PNR/segment)
├─ Flight Level Data.csv              # Flight-level attributes and operational metrics
├─ PNR Remark Level Data.csv          # Raw PNR remarks (textual)
├─ PNR+Flight+Level+Data.csv          # Joined dataset used for modeling & EDA
├─ code.ipynb                         # Jupyter notebook: full pipeline (EDA → features → models)
├─ flight_difficulty_output.csv       # Final predicted flight difficulty / model outputs
└─ README.md                          # (this file)


Contact:
---

Name: Mayank Raj

Email: ironheart.mayank@gmail.com

College: Delhi Technological University (Formerly DCE)
