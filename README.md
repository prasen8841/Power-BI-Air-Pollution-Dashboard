# 🌍 Air Pollution Insights – PM2.5 Trends (2021–2023)

## 📊 Pollution Overview

- **PM2.5** is the dominant pollutant, making up **25.8%** of total pollutants.
- **414 cities** exceeded the WHO PM2.5 limit in **2023**.
- **80%** of cities are above the **WHO-recommended threshold** (5 µg/m³ annual PM2.5).

---

## 📈 Trends & Alarming Increases

- **West Bengal**, **Maharashtra**, **Nagaland**, and **Manipur** show dramatic PM2.5 increases between 2021–2023:
  - 🆘 *West Bengal* saw a **316%** rise.
- Cities like **Begusarai (130.5 µg/m³)** and **Siwan (187 µg/m³)** have PM2.5 levels **>25× the WHO safe limit**.

---

## ✅ Improvement Zones

- **Kerala**, **Jammu & Kashmir**, and **Uttarakhand** show **consistent PM2.5 declines**, suggesting:
  - Effective mitigation strategies.
  - Naturally low pollution environments.

---

## ⚠️ Critical Pollution Spikes

- **Bihar** shows erratic PM2.5 spikes — warrants **close monitoring**.
- **Daman & Diu (UT)** had a **300% jump** in PM2.5 in **2022** — calls for **urgent investigation**.

---

## 🗺️ Regional Comparison

- **North, East, and Central India** are **most affected**.
- **South and Northeast** fare better but not fully safe.
- Even the **least polluted city**, **Lunglei (6.0 µg/m³)**, only *barely* meets WHO standards — a sign of **nationwide concern**.

---

## ✅ Recommendations & Actions

### 1. 🎯 Target High-Risk Zones
- Prioritize top 10 most polluted regions (e.g., **Begusarai, Siwan, West Bengal**).
- Deploy **local sensors** and **micro-monitoring** in areas with **>100 µg/m³ PM2.5**.

### 2. 🚨 Add Visual Red Flags in Dashboard
- Use **WHO PM2.5 thresholds**:
  - `5 µg/m³` (annual)  
  - `15 µg/m³` (daily)
- In Power BI:
  - Show **red bars** in visuals.
  - Add **alert icons** for cities above limits.
  - Use **DAX calculated columns** with **conditional formatting**.

### 3. 🧮 Improve Emissions Reporting
- Use **blank-handling logic** to prevent data dropouts.
- Example DAX:
  ```dax
  AVERAGEX(FILTER(...), [Value])
