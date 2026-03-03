# Hormuz Gas Shock Stress Test on Greek DAM

## Research Question

How sensitive is the Greek Day-Ahead Market (DAM) to a severe natural gas price shock, such as one triggered by a geopolitical disruption (e.g., Strait of Hormuz closure)?

---

## Data

- Hourly Greek DAM MCP (January 2025)
- 744 hourly observations
- Source: HEnEx DAM Results
- Bidding Zone: Mainland Greece

---

## Methodology

1. Identify "gas-like" hours:
   - Defined as the top 25% highest MCP hours (75th percentile threshold).

2. Apply stress-test scenarios to these hours:
   - +50% gas price shock (moderate)
   - +100% gas price shock (severe)
   - +130% gas price shock (extreme scenario based on market stress estimates, e.g., Goldman Sachs)

3. Measure impact on:
   - Average monthly MCP
   - Daily average hours above 200€/MWh (extreme price exposure)

---

## 📈 Results

### Average MCP Impact

| Scenario | Avg MCP (€/MWh) |
|----------|----------------|
| Base | 135 |
| +50% | 159 |
| +100% | 183 |
| +130% | 197 |

Under the extreme +130% scenario, the average DAM price increases by **+45.7%**.

---

### Extreme Price Exposure (>200€/MWh)

Base scenario:
~1.5 high-price hours per day

Extreme scenario:
~6 high-price hours per day

A moderate +50% gas shock already quadruples daily extreme price exposure.

---

## Interpretation

The Greek electricity market shows significant structural exposure to natural gas price shocks.

While average prices increase materially (+45.7% in extreme scenarios), the most critical impact is the amplification of extreme price events, which substantially increases market volatility and risk.

---

## Limitations

- Gas-driven hours identified via statistical proxy (top 25% MCP)
- No direct marginal unit data used
- Simplified linear shock application

This analysis is a stress test, not a price forecast.

---

## Project Structure

- `notebooks/` – analysis notebook
- `figures/` – generated visualizations
