#  Volume-Enhanced Bollinger Bands v2.5  
*TradingView Strategy — Pine Script v6*

---

## Overview  
**Volume-Enhanced Bollinger Bands (VEBB)** is a custom TradingView strategy that augments the classic Bollinger Bands with **volume analytics**, **OBV momentum**, and **adaptive risk controls**.  
It aims to identify high-probability reversals or continuations by combining price volatility and volume behavior.

---

##  Features  
-  **Multi-Layer Volume Confirmation**  
  - Volume Percentile, Z-Score, and Volume Ratio filters  
  - Configurable logic modes: **OR / 2-of-3 / AND**
-  **Adaptive Risk Management**  
  - ATR-based or static % Stop-Loss (SL) and Take-Profit (TP)  
  - Dynamic cooldown based on volatility
-  **Trend Filtering**  
  - 200 EMA filter to confirm trend direction
-  **Momentum Validation**  
  - OBV short-long EMA difference for bullish/bearish strength
-  **Visual & Statistical Tools**  
  - Signal labels and an on-chart performance stats table


---

##  Tech Stack  
- **Language:** Pine Script v6  
- **Platform:** TradingView  
---

##  How It Works  
1. **Signal Generation**  
   - **Buy:** price touches lower Bollinger Band + high volume confirmation + bullish OBV  
   - **Sell:** price touches upper Bollinger Band + high volume confirmation + bearish OBV  
2. **Risk Control**  
   - SL/TP computed via ATR multiples or fixed %.  
3. **Cooldown Logic**  
   - Waits a configurable number of bars (static or adaptive) before allowing new entries.  

---

##  Example Chart  
<img width="762" height="587" alt="image" src="https://github.com/user-attachments/assets/44e06cb4-dc7e-42c5-a22c-f2378858f00b" />

---
