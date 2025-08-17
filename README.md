# 📘 Data Science Assignment – Web3 Trading Team  

**Candidate:** Priyadarshini Singh  

---

## 📑 Project Overview  
This project analyzes the relationship between **trader behavior** (profitability, trade volume, buy/sell patterns) and **market sentiment** (Fear vs Greed).  
By combining **historical trading data** with the **Bitcoin Fear & Greed Index**, the analysis uncovers insights that can support smarter trading strategies in the Web3 ecosystem.  

---

## 📂 Datasets  

1. **Historical Trader Data (`historical_data.csv`)**  
   - Fields: `Account`, `Coin`, `Execution Price`, `Size USD`, `Side`, `Timestamp IST`, `Closed PnL`, etc.  
   - Provides trade-level execution and realized PnL details.  

2. **Fear & Greed Index (`fear_greed_index.csv`)**  
   - Fields: `date`, `classification (Fear/Greed)`, `value`.  
   - Provides daily market sentiment classification.  

---

## 🧠 Methodology  

1. **Data Preprocessing**  
   - Converted timestamps (`Timestamp IST`, `date`) into standard datetime format.  
   - Standardized sentiment classification (`Fear`, `Greed`).  
   - Merged both datasets on `date_only`.  

2. **Exploratory Data Analysis (EDA)**  
   - 📊 Profitability vs Market Sentiment  
   - 📊 Trading Volume vs Sentiment  
   - 📊 Risk Behavior (Buy vs Sell)  

3. **Visualization Outputs** saved in `/outputs`.  

---

## 🔑 Key Findings  

- **Profitability**: Higher during **Greed phases**, while Fear phases showed higher variance in outcomes.  
- **Trading Volume**: More active in Greed, with occasional bursts in Fear (panic selling).  
- **Risk Behavior**:  
  - Greed → more **BUY** orders.  
  - Fear → more **SELL** orders.  
- ⚠️ **Leverage analysis skipped** (not available in dataset).  

---

## 🚀 How to Run  

1. Clone the repository:  
   ```bash
   git clone https://github.com/Priya21darshini/crypto-web3-ds-assignment.git
   cd crypto-web3-ds-assignment
