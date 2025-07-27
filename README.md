# ₿ Cryptocurrency Price Prediction Project

## 👥 Team Project – University of Toronto, Data Science Institute  
**Cohort 5 – Machine Learning – Team 1**  
**Team Members:**  
- Afsaneh Zahmatkesh
- Matias Velastegui
- M.​Hashim Siddiqui
- Soumya Dey
- Zhen Xie 

---

## 📌 Project Objective

Develop a model to **predict the next-day closing price** of a selected cryptocurrency (e.g., Bitcoin or Ethereum) using its historical daily market data.

**This includes:**
- Using features such as daily open, high, low, close, volume, and other derived indicators (e.g., spread, moving averages).
- Predicting a numeric value for tomorrow’s closing price.

**Example Output:**  
> The model predicts that BTC’s closing price tomorrow will be **\$31,750 ± \$120**  
> - \$31,750 = predicted price  
> - ± \$120 = error margin or confidence range

---

## 🎯 Stakeholders & Why They Care

- **Crypto Traders / Investors:** Use predictions to make a profit or avoid losses.
- **Financial Analysts / Portfolio Managers:** Leverage forecasts to optimize portfolio allocations.
- **Data Science Teams:** Validate or build upon forecasting models for financial data.

---

## 📊 Dataset Overview

**Initial Analysis:**
- The dataset includes historical daily market data such as open, high, low, close, volume, and market cap.
- It is fairly clean and usable for time-series modeling but has some limitations.

**Limitations:**
- Lacks external macroeconomic policies or government regulations data.
- Does not include sentiment analysis or news-based signals.
- Political and global events affecting the market are not captured.

---

## ✅ Industry Value Proposition

This project delivers a practical machine learning solution for forecasting cryptocurrency prices in a highly volatile and fast-moving market.

**Value Highlights:**
- **⏱️ Timeliness:** Daily forecasts based on the latest market data.
- **🔍 Transparency:** Each prediction includes a confidence range, not just a point estimate.
- **📈 Scalability:** Can adapt to any coin with historical data, ideal for fintech platforms, analysts, and investors.

> In short: we transform raw crypto market data into **clear, actionable insights** for smarter decision-making.

---

## 📈 Business Question Strategy

**How do we answer our question using the dataset?**

The dataset provides daily price data including:
- Opening price, high, low, close, volume, and market cap for thousands of cryptocurrencies.

**Steps to Model:**
- Clean the data to remove anomalies or missing values.
- Engineer features: lag variables, moving averages, volatility metrics.
- Split into training/testing datasets (e.g., 80/20).
- Train models and evaluate using:
  - **RMSE** (Root Mean Square Error)
  - **MAE** (Mean Absolute Error)
  - **Direction Accuracy** (whether price moved up/down)

> We're not just building a model—we’re **engineering a learning system** to uncover patterns in crypto price movements.

---

## ⚠️ Risks & Uncertainties

- High volatility and unpredictability of the market.
- Incomplete historical or transactional data.
- Excludes external data like regulations, news, or social sentiment.
- Model performance may degrade as market behavior evolves.
- Dataset is at daily frequency—misses intra-day market signals.

> This tool supports decisions, but **does not guarantee accuracy**—especially in unpredictable or news-driven environments.

---

## 🧠 Methods & Technologies

### Model Architectures Considered:

1. **Dense Neural Networks (Fully Connected)**
   - Input → Dense layers (ReLU) → Output (Linear)
   - Best for structured tabular data with numerical/categorical features.

2. **RNNs / LSTM Networks**
   - Input Sequence → LSTM/GRU → Dense Output
   - Suitable for modeling time-series dependencies and temporal signals.

3. **Transformer-Based Models**
   - Input → Multi-head self-attention layers → Dense → Output
   - Excellent for capturing long-term dependencies in large-scale sequential data.

4. **Autoencoders**
   - Input → Encoder → Bottleneck → Decoder → Output
   - Useful for dimensionality reduction and denoising before regression.

---

## 🚀 Future Enhancements

If we had more time, there are several exciting directions we’d explore to extend the project:

- **Multi-Currency Modeling:** Incorporate multiple cryptocurrencies in a unified model to capture interdependencies and market correlations.
- **Sentiment Integration:** Leverage headline news and social media sentiment (e.g., Twitter, Reddit) to enrich the model with real-time public opinion signals.
- **Explainable AI (XAI):** Introduce interpretability tools like SHAP or LIME to help users understand the *why* behind each prediction.
- **Real-Time Prediction API:** Deploy the model via a live API for dynamic, real-time decision-making—moving from analysis to action.


## 🎥 Team Video Links / Deliverables

- [Afsaneh Zahmatkesh]()
- [Matias Velastegui]()
- [M.​Hashim Siddiqui](Team_Videos/presentation-AfsaneZahmatkesh)
- [Soumya Dey](Team_Videos/SoumyaDey.mp4)
- [Zhen Xie]() 
