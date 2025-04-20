# Underdeveloped Countries Classification

[![Python](https://img.shields.io/badge/Python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-0.24.2-green.svg)](https://scikit-learn.org/stable/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

## Overview

This project uses machine learning techniques to classify countries into three categories (underdeveloped, developing, and developed) based on various socioeconomic indicators such as child mortality, exports, health expenditure, imports, income, inflation, life expectancy, birth rate, and GDP.

## Table of Contents

- [Underdeveloped Countries Classification](#underdeveloped-countries-classification)
  - [Overview](#overview)
  - [Table of Contents](#table-of-contents)
  - [Dataset](#dataset)
  - [Features](#features)
  - [Methodology](#methodology)
  - [Project Structure](#project-structure)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Results](#results)

## Dataset

The project uses a dataset (`nation_data.csv`) containing the following features for each country:

- Country name (Ulke)
- Child mortality rate (Cocuk_olumu)
- Export percentage (Ihracat)
- Health expenditure (Saglik)
- Import percentage (İthalat)
- Income (Gelir)
- Inflation rate (Enflasyon)
- Life expectancy (Beklenen_yasam)
- Birth rate (Dogum_sayisi)
- GDP (GSYIH)

## Features

- Data cleaning and preprocessing
- Handling missing values
- Detecting and removing duplicate entries
- Data standardization using Z-score normalization
- Unsupervised learning with K-means clustering
- Classification of countries into three development categories

## Methodology

1. **Data Loading and Exploration**:
   - Load the country dataset
   - Examine column names and structure

2. **Data Cleaning**:
   - Check for missing values
   - Remove rows with missing values
   - Identify and handle duplicate country entries

3. **Data Preprocessing**:
   - Standardize numerical features using Z-score normalization
   - Prepare data for clustering

4. **Clustering**:
   - Apply K-means clustering with k=3
   - Classify countries into three clusters:
     - 0: Underdeveloped countries
     - 1: Developing countries
     - 2: Developed countries

5. **Analysis**:
   - Extract and sort underdeveloped countries
   - Analyze cluster distributions

## Project Structure

```
.
├── underdeveloped_country_selection.ipynb    # Main Jupyter notebook
├── nation_data.csv                         # Country dataset (not included in repo)
└── README.md                                 # Project documentation
```

## Installation

1. Clone this repository
```bash
git clone https://github.com/yourusername/underdeveloped-countries-classification.git
cd underdeveloped-countries-classification
```

2. Install required packages
```bash
pip install pandas numpy scikit-learn jupyter
```

## Usage

1. Launch Jupyter Notebook
```bash
jupyter notebook
```

2. Open the `underdeveloped_country_selection.ipynb` file in the Jupyter interface

3. Run cells sequentially to:
   - Load and clean the dataset
   - Standardize features
   - Perform K-means clustering
   - View classifications

## Results

The project successfully classifies 167 countries into three development categories:
- **Underdeveloped countries (cluster 0)**: 128 countries
- **Developing countries (cluster 1)**
- **Developed countries (cluster 2)**

The final output provides an alphabetically sorted list of underdeveloped countries for further analysis and potential economic development initiatives.

---

Feel free to contribute to this project by submitting pull requests or by reporting issues.