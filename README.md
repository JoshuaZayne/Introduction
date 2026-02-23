# JOSHUA A. T. ZAYNE 👋
### **Head of Multi-Asset Strategies & Systems Architect**
**11 Years of Institutional Quantitative Leadership**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/joshuazayne)
[![Portfolio](https://img.shields.io/badge/Strategy-Portfolio-green?style=flat-square)](https://github.com/JoshuaZayne)

For the past 11 years at **Dimaskus Capital**, I have spearheaded the evolution of our systematic trading and risk infrastructure. My tenure is defined by a transition from a dedicated Quantitative Researcher to the **Head of Multi-Asset Strategies**, where I architect the frameworks that govern our $500M+ multi-asset mandates.

My approach is built on a foundation of **Navy Operational Discipline**. As a former Shift Leader, I translate the "mission-first" mindset into production-grade code, ensuring that every basis point of alpha is generated within a rigorous, audit-ready, and risk-controlled environment.

---

## 🏛️ Institutional Research Pillars

### 1. Systematic Portfolio Architecture
**Production-grade MPT implementation for institutional-scale mandates.**
A scalable Python toolkit for multi-objective optimization, utilizing shrinkage-based covariance estimation to handle institutional frameworks with minimal tracking error.

**[📂 View Portfolio Optimization Library](https://github.com/JoshuaZayne/Efficient_Frontier)**

<details>
<summary><b>📐 View Math: Robust Mean-Variance & Shrinkage</b></summary>

To prevent model instability, I implement **Ledoit-Wolf Shrinkage** on the sample covariance matrix:

$$ \hat{\Sigma}_{LW} = \delta F + (1 - \delta) \hat{\Sigma}_{sample} $$

**Maximum Sharpe Objective Function:**

$$ \max_{w} \frac{w^{T} \mu - r_{f}}{\sqrt{w^{T} \hat{\Sigma}_{LW} w}} $$

**Subject to Constraints:**

$$ \sum_{i=1}^{n} w_{i} = 1, \quad w \geq 0 $$

</details>

---

### 2. Forensic Trade Surveillance Engine
**Algorithmic detection of market abuse across Equities, Options, and Crypto.**
Python-driven logic designed to reconstruct the L2 Order Book and identify non-bona-fide order flow, ensuring 100% compliance with FINRA/SEC "Books and Records" and EBS requirements.

**[📂 View Surveillance Engine](https://github.com/JoshuaZayne/trade-surveillance-engine)**

<details>
<summary><b>📐 View Math: Algorithmic Pattern Recognition</b></summary>

**A. Spoofing/Layering Alert Logic (A):**
Detecting intent through the **Quote-to-Trade Ratio** and **Cancellation Latency** (L):

$$ A = \left( \frac{\sum Orders_{cancelled}}{\sum Trades_{executed}} > \tau \right) \cap (L < 500ms) $$

**B. Wash Trading Probability:**
Matching **Beneficial Ownership IDs** (UBO) across trades with zero change in net market risk:

$$ P(Wash) = \mathbb{I}(UBO_{buy} = UBO_{sell}) \cap (\Delta \beta \approx 0) $$

</details>

---

### 3. Monte Carlo Stress Testing & VaR
**500,000+ simulated paths for multi-asset tail-risk quantification.**
Generates nightly P&L distributions to calibrate VaR/CVaR and ensure model governance aligned with **SR 11-7** standards.

<details>
<summary><b>📐 View Math: Stochastic Risk Projections</b></summary>

**Geometric Brownian Motion (GBM) for Path Generation:**

$$ S_{t+\Delta t} = S_{t} \exp\left[ \left( \mu - \frac{\sigma^{2}}{2} \right) \Delta t + \sigma \sqrt{\Delta t} Z \right] $$

**Conditional VaR (Expected Shortfall) at confidence level alpha:**

$$ CVaR_{\alpha} = \mathbb{E}[ L \mid L \geq VaR_{\alpha} ] $$

</details>

---

### 4. Derivatives Risk & Greeks Decomposition
**Real-time volatility surface fitting and non-linear exposure monitoring.**
Framework for managing complex options books through Greeks tracking and scenario-based stress testing.

**[📂 View Derivatives Framework](https://github.com/JoshuaZayne/black-scholes)**

<details>
<summary><b>📐 View Math: Total Portfolio Risk Sensitivity</b></summary>

To manage non-linear exposures, I decompose portfolio risk across the Greeks surface:

$$ \Delta \Pi \approx \sum_{i=1}^{n} \left( \Delta_{i} \delta S + \frac{1}{2} \Gamma_{i} (\delta S)^{2} + \nu_{i} \delta \sigma + \Theta_{i} \delta t \right) $$

Where **Gamma** captures the acceleration of directional risk and **Vega** quantifies exposure to Implied Volatility shifts.

</details>

---

## 🛠️ The Quantitative Stack

| Domain | Proficiency |
|--------|-----------------|
| **Data Intelligence** | Python (Pandas, NumPy, Scikit-Learn), SQL, ETL Pipeline Automation |
| **Quant Modeling** | MCMC Simulations, GARCH/ARIMA, Black-Scholes, Causal Inference (DiD) |
| **Governance** | SR 11-7 Model Risk Management, GIPS Reporting, Blue Sheet (EBS) Extraction |
| **Infrastructure** | Docker, Git/CI-CD, Bloomberg API, Unit Testing (Pytest) |

---

## 🚀 Impact Track Record

| Pillar | Result |
|---------|--------|
| **Dimaskus Tenure** | 11 years evolving from Quantitative Researcher to Head of Multi-Asset Strategies |
| **Systematic Infra** | Automated $500M+ volume oversight; 85% manual review reduction |
| **Execution Efficiency** | 15bp reduction in transaction costs (TCA) via systematic slippage analysis |
| **Operational Discipline** | Navy Shift Leadership managing 14+ personnel in zero-fail environments |

---

## 📚 Background

**Education**
- **M.S. Finance** — University of Utah, David Eccles School of Business (Exp. 2026)
- **B.S. Quantitative Analysis of Markets & Organizations** — University of Utah (2024)
- **B.S. Applied Mathematics** — University of Utah (2024)

---

## 📫 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/joshuazayne)
[![Email](https://img.shields.io/badge/Email-Inquiry-D14836?style=for-the-badge&logo=gmail)](mailto:joshua.a.zayne@gmail.com)
