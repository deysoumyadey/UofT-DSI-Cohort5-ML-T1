--

# 🧠 UofT-DSI-Cohort5-ML-T1

**Team Project – Machine Learning Team 1 | UofT Data Science Institute (Cohort 5)**

---

## 📌 Project Objective

**Goal:**
Develop a model to predict the **next-day closing price** of a selected cryptocurrency (e.g., Bitcoin, Ethereum) using its historical daily market data.

**Key Tasks:**

* Utilize features such as:
  `Open`, `High`, `Low`, `Close`, `Volume`, and derived indicators (e.g., spread, moving averages).
* Predict a **numeric value** for tomorrow’s closing price.

**Example Output:**

> "The model predicts that BTC’s closing price tomorrow will be **\$31,750 ± \$120**"
>
> * \$31,750 → Predicted Price
> * ± \$120 → Error Margin or Confidence Interval

---

## 🧹 Dataset Cleaning Overview

**Source Dataset:** `crypto-markets.csv` (from [Kaggle](https://www.kaggle.com/datasets/jessevent/all-crypto-currencies))

**Steps Taken:**

* Identified essential columns
* Dropped unused fields
* Defined prediction target as **Next-Day Close Price**

✅ Objective and output format are finalized.

---

## 💼 Business Value & Stakeholders

### 🎯 Who Will Use This?

* **Crypto Traders / Investors**: To make informed buy/sell decisions.
* **Financial Analysts / Portfolio Managers**: For optimizing asset allocation.
* **Data Science Teams**: To benchmark or develop forecasting models.

### 💡 Value to the Industry

* Provides **confidence-backed predictions** to support risk-managed crypto trading.
* Converts raw crypto market data into **actionable insights**.
* Offers a **scalable, transparent solution** built on proven ML architecture.

---

## 🔍 Data Exploration & Limitations

### Is the Data Clean?

* **Mostly clean**, but requires:

  * Removal of anomalies
  * Handling of missing values
  * Verification of consistency in coin identifiers

### Limitations:

* No **policy or regulation features** (e.g., government crypto bans)
* Daily-level data lacks **real-time sentiment signals**
* **High volatility** may affect model reliability

---

## 📈 How We'll Answer the Business Question

Using the Kaggle crypto dataset, we will:

* Preprocess for **clean time-series data**
* Engineer features such as:

  * Lag variables
  * Moving averages
  * Momentum indicators
* Split the dataset (e.g., 80/20) to ensure **temporal validation**
* Train regression models and evaluate using:

  * **RMSE** (Root Mean Square Error)
  * **MAE** (Mean Absolute Error)
  * **Direction Accuracy** (whether price goes up or down)

---

## ⚠️ Risks & Uncertainties

* Crypto market **volatility** and unpredictability
* **Missing or inconsistent** historical data
* Exclusion of **external drivers** (e.g., news, regulations)
* **Model drift** over time as market patterns shift
* Dataset lacks **intraday** data granularity and **sentiment analysis**

---

## 🧠 ML Models Considered

| Model Type                               | Description                                   | When to Use                              |
| ---------------------------------------- | --------------------------------------------- | ---------------------------------------- |
| **Dense Neural Networks (DNN)**          | Input → Dense Layers → Output                 | Great for structured/tabular data        |
| **Recurrent Neural Networks (RNN/LSTM)** | Input Sequence → LSTM/GRU → Dense → Output    | Best for time-series forecasting         |
| **Transformer Models**                   | Input → Transformer Encoders → Dense → Output | Useful for long-range dependencies       |
| **Autoencoders for Regression**          | Input → Encoder → (Decoder) → Output          | Ideal for noisy or high-dimensional data |

---

## 📋 Project Plan (Team Tasks & Contributions)

* Assign **data cleaning**, **feature engineering**, **modeling**, and **evaluation** to team members
* Discuss and implement **cross-validation**, **hyperparameter tuning**, and **error analysis**
* Write up results with **visualizations**, **metrics**, and **business implications**

---

## ✅ Mandatory Team Contributions

1. Each team member must create **at least 1 Pull Request (PR)**.
2. **PR creators cannot merge their own PRs** — another member must **review**, **approve**, and merge.
3. PR reviews must ensure:

   * Code quality and readability
   * Functionality and reproducibility
   * Alignment with the project objective

---

## 📝 TODO List

* [ ] Investigate the **origin of the `rank` column**
  → Suggestion: Try calculating rank from market cap, volume, or other columns and compare.

---

