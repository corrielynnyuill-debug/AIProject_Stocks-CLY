# AIProject_Stocks-CLY
AI Project Stock Predictions

## **Stock Price Analysis & Trading Signal Prediction**  
This repository contains a three‑part machine learning project focused on stock market analysis, technical indicator engineering, and supervised learning for trading signal prediction. The project is implemented in Python using Jupyter Notebooks and Google Colab.

---

## **Project Overview**
The goal of this project is to explore financial time‑series data, engineer technical indicators, and build machine learning models capable of predicting BUY, SELL, and HOLD signals based on market behavior.

The project is divided into three main parts:

---

## ** Part 1 — Data Cleaning & Exploration**
- Loaded raw stock market data  
- Cleaned missing values and inconsistent entries  
- Generated rolling statistics (7‑day, 30‑day averages, volatility)  
- Performed exploratory data analysis (EDA)  
- Saved cleaned dataset to Parquet format  

---

## ** Part 2 — Feature Engineering & Scaling**
- Applied Min‑Max scaling to numerical features  
- Added additional rolling and volatility features  
- Prepared dataset for modeling  
- Saved processed dataset for downstream tasks  

---

## **Part 3 — Technical Indicators & Machine Learning**
- Manually implemented:
  - **MACD** (12/26 EMA + 9‑period signal line)  
  - **RSI** (EMA‑based gain/loss calculation)  
- Generated BUY/SELL/HOLD labels based on indicator behavior  
- Balanced the dataset to address class imbalance  
- Trained three ML models:
  - Logistic Regression  
  - Random Forest Classifier  
  - Support Vector Machine (SVM)  
- Evaluated models using accuracy, precision, recall, F1‑score, and confusion matrices  
- Discussed limitations and insights related to financial prediction  

---

## **Repository Structure**
```
├── part1_data_cleaning.ipynb
├── part2_feature_engineering.ipynb
├── part3_modeling_and_signals.ipynb
├── README.md
```

---

## **Technologies Used**
- Python  
- Pandas, NumPy  
- Scikit‑Learn  
- Matplotlib, Seaborn  
- Google Colab  
- Parquet file format  

---

## **Key Insights**
- Technical indicators like MACD and RSI rarely align perfectly, resulting in few BUY/SELL signals.  
- Class imbalance is a major challenge in financial ML tasks.  
- Random Forest performs well on small balanced datasets but may overfit.  
- Logistic Regression and SVM provide more stable generalization but require more signal density.  
- Expanding to multiple tickers or loosening signal rules would improve predictive performance.  

---

## ** License**
This project is for educational and research purposes.

