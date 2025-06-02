
# 📈 US Large-Cap Stock Price Analysis (2015–2025)

**Author:** Adhiraj Karjee
**Entry No:** 2024HES7241
**Institution:** IIT Delhi
**Domain:** Time-Series Analysis, Financial Analytics, Python (Pandas, Matplotlib)

---

## 🔍 Project Overview

This project performs structured exploratory data analysis and time-series transformation on historical daily price-volume data for five large-cap US companies — **AAPL**, **AMZN**, **GOOGL**, **MSTR**, and **ABBV** — using Python.
Data is processed, cleaned, and transformed to compute daily returns, moving averages, and rolling volatility, followed by visual and statistical analysis.

---

## 🗂️ Dataset Details

* **Source Format:** `.txt` files (one per ticker)
* **Columns:** `Date`, `Open`, `High`, `Low`, `Close`, `Volume`, `OpenInt`
* **Time Horizon:** Full historical data filtered to the **last 10 years**

---

## 🛠️ Key Steps

### ✅ Step 1: Data Loading & Structuring

* Load `.txt` data files from local paths.
* Create a **MultiIndexed DataFrame** with `Ticker` and `Date` as index levels.
* Sort index chronologically within each ticker.

### ✅ Step 2: Data Cleaning

* Forward-fill & backward-fill missing data per ticker.
* Ensure proper `datetime` formatting of the index.
* Filter dataset to include only data from **June 2, 2015, onward**.

### ✅ Step 3: Feature Engineering

* **Daily Return** (%)
* **7-day & 30-day Moving Averages**
* **Rolling Volatility (30-day window)**

### ✅ Step 4: Exploratory Analysis

* Plot closing prices of all stocks over the last 10 years.
* Identify:

  * Ticker with **highest average return**: `AMZN`
  * Ticker with **maximum volatility**: `MSTR`, in **August 2017** (4.94%)

---

## 📊 Visualizations

* Line plots of closing prices (2015–2025) per ticker
* Rolling volatility trends
* Moving averages superimposed on price charts

---

## 📈 Key Findings

| Metric                     | Ticker | Value             |
| -------------------------- | ------ | ----------------- |
| 📈 **Highest Avg Return**  | AMZN   | 0.170%            |
| ⚡ **Most Volatile Period** | MSTR   | 4.94% in Aug 2017 |
| 🔒 **Least Volatile**      | AAPL   | Relatively stable |

---

## 🧰 Tech Stack

* **Python**: Data wrangling and analysis
* **Pandas**: MultiIndexing, transformation, aggregation
* **Matplotlib**: Time-series plotting

---

## 📎 How to Run

1. Clone this repo
2. Place your `.txt` files in the `/data/` directory
3. Modify the `file_paths` dictionary in the script to match your system
4. Run the notebook or Python script


---

## 📜 License

This project is for educational and non-commercial research use only.
