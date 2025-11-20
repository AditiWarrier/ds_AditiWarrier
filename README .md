# README
# Bitcoin Market Sentiment vs Trader Behavior Analysis  
**Author:** Aditi Warrier  
**Date:** February 2025  



## 1. Overview  

This project analyzes how trader behavior (profitability, volume, risk, win rate, and consistency) changes across different Bitcoin market sentiment regimes such as Fear, Neutral, and Greed.  
The goal is to determine whether trader performance moves with sentiment, moves against it, or remains independent — and to extract insights that may support better trading strategies.

This README includes setup instructions, folder structure, and notes for running the project.



## 2. Folder Structure
ds_AditiWarrier/
│
├── notebook_1.ipynb
├── outputs/
│     ├── sentiment_distribution.png
│     ├── avg_pnl_by_sentiment.png
│     ├── avg_volume_by_sentiment.png
│     ├── correlation_heatmap.png
│     ├── pnl_outlier_analysis.png
│     ├── rolling_averages.png
│     ├── sentiment_shock_timeline.png
│     └── pnl_distribution_by_sentiment.png
│
├── data/
│     ├── historical_data.csv
│     └── fear_greed_index.csv
│
└── ds_report.pdf  


## Google Colab Notebook
The full analysis code can be viewed in Google Colab here:  
👉 **https://colab.research.google.com/drive/1NjgX2KjKyPPPoqIQDoBl3Sh_Rky4zmQn?usp=sharing**

**Access Requirement:** Set to *"Anyone with the link can view"*.




## 3. Setup Instructions  

The analysis was originally executed in **Google Colab**.

To run locally, install:

- Python 3.8+
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scipy  
- scikit-learn  
- statsmodels  

Install all at once:

```
pip install pandas numpy matplotlib seaborn scipy scikit-learn statsmodels
```



## 4. How to Run the Analysis  

### **Step 1 — Download the Project Folder**  
Copy the entire `ds_AditiWarrier` folder to your working environment.

### **Step 2 — Open `notebook_1.ipynb`**  
Use Google Colab or Jupyter Notebook.

### **Step 3 — Place CSV Files in the `data/` Folder**  
Required files:

- `historical_data.csv`  
- `fear_greed_index.csv`  

### **Step 4 — Run All Cells**  
The notebook will automatically run:

- Data loading  
- Cleaning & preprocessing  
- Merging sentiment with trader activity  
- Exploratory data analysis  
- Statistical tests  
- Clustering (K-Means)  
- Trader-level metrics  
- Risk & sentiment shock analysis  
- Final summary  

All graphs will be saved to the **outputs/** directory.



## 5. Summary of Workflow  

### **Data Preparation**  
- Standardized timestamps  
- Daily aggregation of PnL, volume, fees  
- Merged with sentiment data  

### **Exploratory Data Analysis (EDA)**  
- Sentiment distribution  
- Average PnL by sentiment  
- Volume trends  
- Correlation heatmap  
- Outlier detection  
- Rolling 5-day behavior patterns  
- Sentiment shock visualization  

### **Advanced Analysis**  
- K-Means clustering for trader segmentation  
- Sharpe-like risk-adjusted returns  
- Win rate and consistency scores  
- Trader rankings  
- Contrarian trader detection  
- Maximum drawdown  
- PnL response to sentiment shocks  

### **Final Output**  
- All graphs saved in `outputs/`  
- Full written analysis in `ds_report.pdf`  



## 6. Notes  

- The analysis focuses on **interpretable metrics**, not algorithmic trading models.  
- Sentiment data is **daily**, so intraday effects are not captured.  
- Insights are based on ~480 days and 32 traders, which limits generalization.  



## 7. Contact  

For questions or clarifications, email:  
**aditisw02@gmail.com**
