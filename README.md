# 📊 Stock Price & Tweet Sentiment Analysis

![Python](https://img.shields.io/badge/python-3.12-blue)
![License](https://img.shields.io/badge/license-MIT-green)

Analyze how **Twitter sentiment** relates to **stock price changes** for 25 major companies.  
This project combines **NLP sentiment analysis** and **stock market data** to test whether tweets can predict short-term price movements.  

---

## 📂 Setup Instructions

Clone the repository and set up a virtual environment:

```bash
git clone https://github.com/your-username/embrizon_project_1.git
cd embrizon_project_1
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

If `requirements.txt` is missing, install manually:

```bash
pip install numpy pandas matplotlib seaborn nltk statsmodels scikit-learn jupyter
```

---

## 🔄 How to Use

1. Open the notebook in **Jupyter**:
   ```bash
   jupyter notebook embrizon_project_1.ipynb
   ```  
2. Run all cells **top to bottom**.  
3. Outputs include:  
   - Correlation heatmap (per stock).  
   - Sentiment vs price plots (dual-axis).  
   - Summary statistics of correlations.  

---

## 📊 Dataset

This project uses two datasets:  
- **embrizon_project_1.csv** → Tweets with stock ticker tags.  
- **stock_yfinance_data.csv** → Daily adjusted close prices from Yahoo Finance.  

After merging, the **processed dataset (`merged_dataset.csv`)** contains:  
- Date, Stock Name, Tweet, Sentiment Score, Adj Close, Price Change.  

---

## 📈 Key Results

- 📉 **Weak overall relationship** → most tweet–price pairs showed **no clear correlation** (~44k cases).  
- 📊 **Correlation never exceeds 0.21** → even in volatile markets, the sentiment-price link is weak.  
- 🐦 **Tweet volume doesn’t help** → more tweets ≠ stronger correlation.  
- 📉 **Visual analysis** → sentiment trends (e.g., TSLA, AAPL, TSM) often diverge from price trends.  

Example visualizations:  
![Correlation Heatmap](docs/correlation_heatmap.png)  
![Sentiment vs Price](docs/sentiment_vs_price.png)  

---

## 🛠️ Tech Stack

- **Python** 🐍  
- **Pandas / NumPy** → Data handling  
- **NLTK (VADER)** → Sentiment analysis  
- **Matplotlib / Seaborn** → Visualization  
- **Statsmodels** → Time-series tools  
- **Scikit-learn** → ML utilities  
- **Jupyter Notebook** → Interactive workflow  

---

## 🤝 Contributing

Pull requests are welcome!  
- Fork the repo  
- Create a feature branch (`git checkout -b feature-name`)  
- Commit changes and open a Pull Request  

---

## 📜 License

This project is licensed under the **MIT License**.  

---

📌 **Author:** *Shivam Amitbhai Patel*
