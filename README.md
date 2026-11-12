# OMNIUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **OMNIUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `OMNIUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `18` months
- **Total Candles:** `762,660` 1-minute candles
- **Historical Range:** `2024-04-17 12:00:00` to `2025-09-29 02:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
OMNIUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── OMNIUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/OMNIUSDT-Historical-Data/main/1m/2026/11/OMNIUSDT_1m_2026-11.csv"
df = pd.read_csv(url)
print(df.head())
```
