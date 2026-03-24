# Core-Strategic-Modeling
Central repository for MVSM (Non-linear Risk Audit Protocol) | Phase 2: Stress Testing & Data Integration

# MVSM Oil Risk Auditor (v12.0)
> **A State-Space Model for Geopolitical Risk Auditing**

## Overview
This repository contains the **MVSM 12.0** engine, designed to audit the energy market impacts of the **March 28, 2026 Geopolitical Ultimatum**. 

Unlike linear forecasting tools, MVSM simulates the **Closed-loop Dynamics** of Flow-Stock-Price, capturing non-linear "Price Singularities" during inventory depletion.

## Key Features
- **Poisson Jump Process**: Simulates discrete geopolitical shocks.
- **Inventory Buffer**: Tracks global stock levels as a shock absorber.
- **Demand Feedback**: Incorporates price-induced demand destruction.
- **Monte Carlo Simulation**: 5,000+ parallel paths to identify "Fat-tail" risks.

## Mathematical Framework
The model follows the state-space evolution:
1. **Flow**: $\Delta S_t = (Gap_{init} - \eta(P_t - \bar{P}) + J \cdot \mathbb{1}_{event})$
2. **Stock**: $I_{t+1} = I_t - \Delta S_t$
3. **Price**: $P_{t+1} = P_t + (\alpha \cdot \Delta S_t \cdot e^{\frac{I_{crit} - I_t}{\sigma}}) + \epsilon_t$

## Usage
Run `audit_dashboard.ipynb` in a Jupyter environment to interact with the model parameters.