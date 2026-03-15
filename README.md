# Sepedi Rabies Awareness Chatbot

This repository contains the dataset and exploratory data analysis (EDA) for the
MIT 808 Capstone Project at the University of Pretoria. The project focuses on
preparing and analysing a bilingual Sepedi–English rabies awareness dataset for
use in a chatbot.

---

## Project Description

Rabies is a fatal but preventable disease, yet language barriers limit access to
health information in many rural South African communities. This project builds
on earlier work by De Wet & Govender (2025) and provides a cleaned, versioned
dataset of rabies-related question–answer pairs in Sepedi and English.

The dataset contains 110 bilingual Q&A pairs across six topics:
- Epidemiology
- Prevention
- Virology
- Clinical signs
- Geography / risk areas
- Public awareness

Translations are versioned (v1 and v2) to document corrections, terminology
refinement, and completeness improvements.

---

## Repository Structure

.
├── data/
│   ├── raw/              # Original Excel files
│   └── processed/        # Combined CSV for analysis and chatbot use
├── notebooks/
│   └── EDA_Sepedi_Rabies.ipynb   # Exploratory data analysis
├── figures/              # Generated plots and visualisations
├── requirements.txt      # Python dependencies
└── README.md

---

## Dataset

The dataset is publicly available on Kaggle:
https://www.kaggle.com/datasets/muphulusi1234/rabies

It consists of 14 Excel files, including main topic files and additional test
translations. The analysis uses the 12 files prefixed with `rabies_topic*`.

### Dataset Summary
- 110 bilingual Sepedi–English Q&A pairs
- 6 topic categories
- Versioned translations (v1 / v2)
- 99.4% complete
- 2 missing English translations in topic3_v1 (resolved in v2)
- Average Sepedi question length: 68 characters
- Average Sepedi answer length: 106 characters

---

## Exploratory Data Analysis (EDA)

The EDA is implemented in a Jupyter notebook and includes:
- Data loading and inspection
- Missing value analysis
- Text length statistics
- Topic coverage
- Version comparison (v1 vs v2)
- Medical terminology frequency
- Visualisations (distributions, bar charts, word cloud)

Colab notebook:
https://colab.research.google.com/drive/1OV79SKBKs_UDqsDsdufJcJbHQCrjh0xl

---

## Running the Analysis

Install dependencies:
pip install -r requirements.txt

Clone the repository:
git clone https://github.com/MuphulusiDzivhani/Rabies-chatbot.git
cd Rabies-chatbot

Run the notebook:
Open notebooks/EDA_Sepedi_Rabies.ipynb and execute all cells.

The processed dataset (sepedi_rabies_combined.csv) is saved in:
data/processed/

---

## Key Findings

- The dataset is clean and structured for downstream use.
- Version 2 files show clear improvements in translation quality and completeness.
- Medical terminology is mostly consistent, but expert validation is recommended
  for terms such as PEP and PrEP.
- The Epidemiology topic has fewer entries and may require supplementation using
  WHO or NICD materials.

---

## Credits

- Dr Tedson Nkoana (Future Africa, University of Pretoria) – dataset provision and supervision
- National Institute for Communicable Diseases (NICD) – source educational material
- De Wet & Govender (2025) – preliminary translation work
- Muphulusi Dzivhani & Nonhlanhla Mabila – MIT 808 students, EDA and repository authors

---

## License

The dataset is derived from public health educational materials and is intended
for academic and research use. Please cite appropriately.

---

## Contributing

Issues and pull requests are welcome if they improve data quality,
documentation, or analysis clarity.
