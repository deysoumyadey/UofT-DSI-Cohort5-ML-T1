---

# UofT-DSI-Cohort5-ML-T1

Team project for UofT-DSI cohort 5 Machine Learning Team 1

---

## 📌 Project Objective

Develop a model to predict the next-day closing price of a selected cryptocurrency (e.g., Bitcoin or Ethereum) using its historical daily market data.

This includes:

* Using features such as daily open, high, low, close, volume, and other derived indicators (e.g., spread, moving averages)
* Predicting a numeric value for tomorrow’s closing price

**Example output:**
The model predicts that BTC’s closing price tomorrow will be **\$31,750 ± \$120**

* \$31,750 = predicted price
* ± \$120 = error margin or confidence range

---

## 🧹 Clean dataset (crypto-markets.csv)

* Identify essential columns
* Drop unused fields
* Define the prediction target (next-day close)
* Objective and example output ready

---

## 🔍 Dig deeper into your business question to understand the value you will be delivering

**Who are your stakeholders and why do they care about your project?**
**Ans:**

* Crypto Traders / Investors: Use predictions to make a profit or avoid a loss.
* Financial Analysts / Portfolio Managers: Use forecasts to optimize allocations.
* Data Science Teams: Interested in building or validating models

---

## 📊 Explore your dataset

**Is it clean? What are its limitations? Will you be able to answer your question with this dataset?**
**Start your analysis:**

* Policy is missing, e.g. govt. mandates towards the transaction

---

## 📁 Add your project plan to your team's README file

This plan should include details on:

### ✅ What value does your project bring to the industry?

* Leverages machine learning to deliver accurate, next-day price predictions for top cryptocurrencies.
* Turns raw market data into clear, actionable insights—built for speed, simplicity, and scalability.
* Empowers traders with transparent, confidence-backed forecasts to manage risk and maximize opportunity.

---

### 📈 How will you answer your business question with your chosen dataset?

**Answer:**
The dataset from Kaggle provides information about the price daily data for thousands of coins, including: Opening price, High and low price, Volume, Market capitalization, and Closing price. We will:

* ensure clean time-series data with no missing or anomalous values
* create features that help capture temporal patterns (e.g., lag variables, moving averages, momentum indicators)
* split the data into training and testing sets (e.g., 80/20 split), using only historical data to predict the future price
* then train a predictive model and evaluate its performance using metrics such as RMSE (Root Mean Square Error), MAE (Mean Absolute Error), and direction accuracy (whether the price went up or down)

---

### ⚠️ What are the risks and uncertainties?

* High market volatility and unpredictability
* Missing or inconsistent historical data
* Excludes external factors (e.g., news, regulations)
* Market behavior may change over time
* Limited accuracy in short-term forecasting
* Lacks fine-grained market sentiment, as the dataset provides only daily-level data

---

### 🧠 What methods and technologies will you use?

**Model Examples to Consider:**

1. **Dense Neural Networks (Fully Connected Networks)**
   Architecture: Input layer → Multiple dense (fully connected) layers with activation functions (e.g., ReLU) → Output layer (linear activation for regression).
   **When to Use:** Suitable for structured data like numerical or categorical features (e.g., predicting house prices based on features like size and location).

2. **Recurrent Neural Networks (RNNs) / Long Short-Term Memory (LSTM) Networks**
   Architecture: Input (sequence) → LSTM/GRU layers → Dense layers → Output (linear).
   **When to Use:** Best for time-series regression, such as forecasting sales or predicting energy consumption based on historical data.

3. **Transformer-Based Models for Regression**
   Architecture: Input → Transformer encoder layers (multi-head self-attention) → Dense layers → Output (linear).
   **When to Use:** Useful for complex sequential data or when capturing long-range dependencies (e.g., predicting trends in large time-series datasets).

4. **Autoencoders for Regression**
   Architecture: Input → Encoder (dense/conv layers) → Bottleneck → Decoder (optional) → Dense output (linear).
   **When to Use:** Effective for regression with noisy or high-dimensional data, such as denoising sensor data or predicting values from compressed representations.

---

## 👥 Assign data cleaning and analysis tasks to team members

---

## ✅ TODO

1. Find the origin of rank. Suggestion: Try to calc rank from different columns and check if they match with the given rank.

---

## 📌 Mandatory contributions towards the project

1. Everyone creates at least 1 Pull request.
2. Person creating the PR won't merge the PR, someone else will verify, approve, and (may\*) merge.
3.

---
