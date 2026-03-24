# Simulation Results and Analysis

This document contains the simulation results derived from the MVSM 12.0 Monte Carlo analysis executed on March 28, 2026.

## Simulation Parameters

- **Initial Price:** $112/barrel
- **Supply Gap:** 1.50 mb/d
- **Event Intensity:** 0.30
- **Global Stock Buffer:** 45 days
- **Number of Simulations:** 5,000 Monte Carlo paths

## Results Visualization

![MVSM 12.0: Monte Carlo Price Distribution @ March 28](https://github.com/Michael-Xie-Risk-Analyst/MVSM-Public-Demo/blob/6183a231c546102710c720ae2d194588b079f3f2/results/image.png, https://github.com/Michael-Xie-Risk-Analyst/MVSM-Public-Demo/blob/6183a231c546102710c720ae2d194588b079f3f2/results/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202026-03-24%20162536.png)

## Key Insights

### Critical Risk Metric
- **Logic Rupture Probability (Price > $150):** 14.12%

This indicates that under current market conditions, there is approximately a 1-in-7 chance of the system experiencing a critical rupture event within the simulation timeframe.

### Price Distribution Analysis

The histogram above illustrates the probability density of terminal prices across 5,000 simulated scenarios:

- **Distribution Shape:** The prices follow a roughly normal distribution centered around $120-$130
- **Rupture Zone (Red Shaded Area):** Prices exceeding $150/barrel represent a critical threshold where supply-demand dynamics could destabilize
- **Tail Risk:** Approximately 14% of scenarios result in prices entering the rupture zone

### Implications

1. **Market Stability:** With the current gap and intensity parameters, the market has an 86% probability of remaining stable
2. **Risk Concentration:** The 14% rupture probability is concentrated in the right tail of the distribution
3. **Buffer Adequacy:** The 45-day stock buffer provides moderate insulation but is insufficient to prevent all rupture scenarios
4. **Geopolitical Sensitivity:** The 0.30 intensity factor reflects moderate geopolitical risk; higher intensity values would increase rupture probability

## Methodology

The MVSM (Multidimensional Vector Supply Model) 12.0 employs:
- Monte Carlo simulation with 5,000 paths
- Stochastic modeling of supply disruptions
- Dynamic price discovery mechanisms
- Inventory depletion dynamics

## Conclusion

The analysis demonstrates that while the market maintains reasonable stability under current conditions (86% no-rupture probability), the 14% rupture risk warrants active monitoring of supply gap dynamics and geopolitical developments.
