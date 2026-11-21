# Week 1: Data Gathering, Cleaning and Preprocessing

## Overview
Cleaning and preprocessing of the UCI Online Retail dataset (transactions from a UK online retailer, 2010–2011).

## Dataset
Source: https://archive.ics.uci.edu/dataset/352/online+retail
Raw size: <ROWS> rows × 8 columns

## What was done
- Explored structure, types and summary statistics
- Removed <N> duplicate rows
- Handled missing Description (dropped) and CustomerID (labelled "Unknown")
- Removed cancellations and invalid quantities/prices
- Converted data types, engineered TotalPrice, Month, Hour
- Capped outliers using the IQR method
- Applied Min-Max normalization and standardization
Final dataset: <ROWS> rows × <COLS> columns

## Project structure
data/raw/       original dataset
data/cleaned/   cleaned CSV
notebooks/      cleaning.ipynb
report/         report (.docx and .pdf) and figures

## How to run
1. python -m venv venv and activate it
2. pip install pandas numpy matplotlib seaborn scikit-learn openpyxl ipykernel
3. Place Online Retail.xlsx in data/raw/
4. Run notebooks/cleaning.ipynb from top to bottom