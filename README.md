## Trader Behavior vs Market Sentiment Analysis ##
 # Overview

This project analyzes the relationship between **Bitcoin market sentiment (Fear/Greed)** and **trader behavior & performance** using historical trading data from Hyperliquid.

The goal is to uncover actionable insights that can inform smarter trading strategies.

---

## Objectives

* Analyze how **market sentiment impacts trader performance (PnL, win rate)**
* Study **behavioral changes** (trade frequency, leverage, long/short bias)
* Identify **trader segments** (high vs low frequency, large vs small trades)
* Propose **data-driven trading strategies**

---

## Dataset Details

### 1. Bitcoin Market Sentiment

* Columns: `date`, `classification` (Fear / Greed)

### 2. Historical Trader Data

* Columns include:

  * `account`
  * `symbol`
  * `execution price`
  * `size`
  * `side` (long/short)
  * `timestamp`
  * `closedPnL`
  * `leverage`

---
##  Dataset Access

The datasets used in this project are provided by the assignment and can be downloaded from the following links:

* [Bitcoin Market Sentiment Dataset](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)
* [Historical Trader Data (Hyperliquid)](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing)

Please download the datasets and place them in the project directory before running the notebook.

Note: Due to file size constraints, datasets are not included in this repository.


##  Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/trader-sentiment-analysis.git
cd trader-sentiment-analysis
```

### 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn
```

### 3. Add Datasets

Download datasets and place them in the project folder:

* `sentiment.csv`
* `trades.csv`

---

##  How to Run

### Option 1: Jupyter Notebook


jupyter notebook

* Open `Trader_Sentiment_Analysis.ipynb`
* Run all cells sequentially

### Option 2: Google Colab

* Upload the notebook
* Mount Google Drive (if needed)
* Update dataset file paths

---

##  Workflow

1. **Data Loading**
2. **Data Cleaning & EDA**

   * Missing values
   * Duplicates
3. **Data Alignment**

   * Convert timestamps
   * Merge datasets by date
4. **Feature Engineering**

   * Win rate
   * Daily PnL
   * Trade frequency
5. **Segmentation**

   * High vs Low frequency traders
   * Large vs Small trades
6. **Analysis**

   * Performance vs sentiment
   * Behavioral changes
7. **Insights & Strategy**

---

##  Key Insights

* Traders perform **better during Greed periods** compared to Fear periods
* **High-frequency traders** tend to maintain more stable performance
* Traders show a **long bias during Greed** and **short bias during Fear**
* High leverage during Fear leads to **higher losses**

---

##  Strategy Recommendations

* Reduce leverage during **Fear periods**, especially for high-frequency traders
* Increase participation during **Greed periods** with controlled risk
* Avoid overtrading during volatile sentiment shifts
* Use sentiment as a **signal for directional bias (long/short)**

---

##  Tech Stack

* Python 
* Pandas
* NumPy
* Matplotlib / Seaborn
* Colab Notebook

---

##  Project Structure

```bash
├── Trader_Sentiment_Analysis.ipynb
├── sentiment.csv
├── trades.csv
├── README.md

---

##  Author

Gopika GK
(Data Science Enthusiast)
