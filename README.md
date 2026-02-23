# JOSHUA A. T. ZAYNE 👋
### **Quantitative Strategist & Systems Architect**
**Bridging Fiduciary Stewardship with Algorithmic Integrity**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/joshuazayne)
[![Portfolio](https://img.shields.io/badge/Strategy-Portfolio-green?style=flat-square)](https://github.com/JoshuaZayne)

I spent a decade in the **U.S. Navy Reserves** as a Shift Leader, developing the operational discipline required to lead technical teams in zero-fail environments. Today, I translate that "mission-first" mindset into the architecture of systematic trading strategies and forensic risk engines as **Head of Multi-Asset Strategies** at Dimaskus Capital.

My work centers on the **"Poacher-turned-Gamekeeper"** philosophy: utilizing a deep understanding of market microstructure and portfolio optimization to build the next generation of automated surveillance and risk-management frameworks.

---

## 🏛️ Executive Research Pillars

### 1. Systematic Portfolio Architecture
**Production-grade MPT implementation for institutional-scale mandates.**
A scalable Python toolkit for multi-objective optimization, utilizing shrinkage-based covariance estimation to handle $500M+ AUM frameworks with minimal tracking error.

**[📂 View Portfolio Optimization Library](https://github.com/JoshuaZayne/Efficient_Frontier)**

<details>
<summary><b>📐 The Math: Robust Mean-Variance & Ledoit-Wolf Shrinkage</b></summary>

To prevent model instability and "error maximization," I implement **Ledoit-Wolf Shrinkage** on the sample covariance matrix:

$$
\hat{\Sigma}_{LW} = \delta \mathbf{F} + (1-\delta) \hat{\Sigma}_{\text{sample}}
$$

**Maximum Sharpe Objective Function:**

$$
\max_{\mathbf{w}} \frac{\mathbf{w}^\top \boldsymbol{\mu} - r_f}{\sqrt{\mathbf{w}^\top \hat{\Sigma}_{LW} \mathbf{w}}}
$$

**Subject to Constraints:**

$$
\sum_{i=1}^{n} w_i = 1, \quad \mathbf{w} \geq 0
$$

*This approach ensures that the resulting efficient frontier is resilient to the estimation noise prevalent in high-volatility market regimes.*
</details>

---

### 2. Forensic Trade Surveillance Engine
**Algorithmic detection of market abuse across Equities, Options, and Crypto.**
Python-driven logic designed to reconstruct the L2 Order Book and identify non-bona-fide order flow, ensuring 100% compliance with FINRA/SEC "Books and Records" and EBS requirements.

**[📂 View Surveillance Engine](https://github.com/JoshuaZayne/trade-surveillance-engine)**

<details>
<summary><b>📐 The Math: Algorithmic Pattern Recognition</b></summary>

**A. Spoofing/Layering Alert Logic ($A$):**
Detecting intent through the **Quote-to-Trade Ratio** and **Cancellation Latency** ($\mathcal{L}$):

$$
A = \left( \frac{\sum \text{Orders}_{\text{cancelled}}}{\sum \text{Trades}_{\text{executed}}} > \tau \right) \cap (\mathcal{L} < 500\text{ms})
$$

**B. Wash Trading Probability:**
Matching **Beneficial Ownership IDs** ($UBO$) across trades with zero change in net market risk ($\Delta \beta$):

$$
P(\text{Wash}) = \mathbb{I}(UBO_{\text{buy}} = UBO_{\text{sell}}) \cap (\Delta \beta \approx 0)
$$
</details>

---

### 3. Monte Carlo Stress Testing & VaR
**500,000+ simulated paths for multi-asset tail-risk quantification.**
Generates nightly P&L distributions to calibrate VaR/CVaR and ensure model governance aligned with **SR 11-7** standards.

<details>
<summary><b>📐 The Math: Stochastic Risk Projections</b></summary>

**Geometric Brownian Motion (GBM) for Path Generation:**

$$
S_{t+\Delta t} = S_t \exp\left[\left(\mu - \frac{\sigma^2}{2}\right)\Delta t + \sigma \sqrt{\Delta t} \, Z\right], \quad Z \sim \mathcal{N}(0,1)
$$

**Conditional VaR (Expected Shortfall) at confidence level $\alpha$:**

$$
\text{CVaR}_{\alpha} = \mathbb{E}[L \mid L \geq \text{VaR}_{\alpha}]
$$

*Utilized to ensure institutional portfolios remain within predefined risk-appetite constraints during black-swan events.*
</details>

---

### 4. Derivatives Risk & Greeks Decomposition
**Real-time volatility surface fitting and non-linear exposure monitoring.**
Framework for managing complex options books through millisecond Greeks tracking and scenario-based stress testing.

**[📂 View Derivatives Framework](https://github.com/JoshuaZayne/black-scholes)**

<details>
<summary><b>📐 The Math: The Black-Scholes Greeks Surface</b></summary>

**Total Portfolio Risk Sensitivity:**

$$
\Delta \Pi \approx \sum_{i=1}^{n} \left( \Delta_i \delta S + \frac{1}{2}\Gamma_i (\delta S)^2 + \nu_i \delta \sigma + \Theta_i \delta t \right)
$$

Where $\Gamma$ captures the "acceleration" of directional risk and $\nu$ quantifies exposure to the 1st-order move in Implied Volatility.
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

## 🚀 Recent Impact Track Record

| Pillar | Result |
|---------|--------|
| **Systematic Infrastructure** | Automated $500M+ volume oversight; 85% manual review reduction |
| **Execution Efficiency** | 15bp reduction in transaction costs (TCA) via systematic slippage analysis |
| **Surveillance Precision** | 37% improvement in alert precision via statistical thresholding |
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
