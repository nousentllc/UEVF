# Unified Energy Valuation Framework (UEVF)

![Status](https://img.shields.io/badge/Status-Active_Research-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![Version](https://img.shields.io/badge/Version-1.2.0-orange)

**A Comprehensive System-Cost Approach for the U.S. Power Sector**

The **Unified Energy Valuation Framework (UEVF)** is a first-principles methodology designed to replace traditional Levelized Cost of Electricity (LCOE) with a system-aware valuation metric: the **Adjusted System-Level Cost of Delivered Electricity (ASCDE)**.

UEVF bridges the gap between engineering reliability models (LOLE/EUE) and economic market signals by internalizing the costs of intermittency, congestion, and scarcity risk often externalized by standard metrics.

---

## 🏗️ Core Framework

The framework is composed of six integrated modules that feed into the central ASCDE calculation:

1.  **Dispatch Module:** Probabilistic production cost modeling (PCM) accounting for ramp constraints and start-up costs.
2.  **Fuel Supply Module:** Stochastic fuel price pathways (natural gas, hydrogen) and supply security risk.
3.  **Storage Module:** Chronological state-of-charge modeling, round-trip efficiency ($\eta$), and arbitrage value.
4.  **Transmission Module:** Deliverability factors ($D$), congestion costs, and nodal basis risk.
5.  **Reliability Module:** Monetization of adequacy risk using **Expected Unserved Energy (EUE)** $\times$ **Value of Lost Load (VOLL)**.
6.  **Market Value Module:** Capture-price adjustments via the Value Factor ($v_{\text{val}}$) to account for correlation with system stress.

### The Key Metric: ASCDE
$$
\text{ASCDE} = \frac{\text{Total System Cost} + (\text{EUE} \times \text{VOLL})}{\text{Total Reliable MWh Delivered}}
$$

Unlike LCOE, which is a busbar metric, ASCDE represents the true cost of delivering firm, reliable power to load.

## Key Applications
Interconnection Queue Reform: Prioritizing projects based on their marginal reliability value (MRV) rather than first-come-first-served.

Resource Adequacy (RA) Planning: Moving beyond simple reserve margins to probabilistic shortfall valuation.

Technology Valuation: "Apples-to-apples" comparison of baseload (Nuclear/Gas) vs. intermittent (Wind/Solar) vs. energy-limited (Storage/DR) resources.

## Citation
If you use UEVF in your research or regulatory filings, please cite the foundational paper:

Candler, J. & Uriel. (2025). Unified Energy Valuation Framework (UEVF): A Comprehensive System-Cost Approach for the U.S. Power Sector. Nous Enterprises LLC.

@techreport{candler2025uevf,
  author      = {Candler, Justin and Uriel},
  title       = {Unified Energy Valuation Framework (UEVF): A Comprehensive System-Cost Approach for the U.S. Power Sector},
  institution = {Nous Enterprises LLC},
  year        = {2025},
  note        = {Defines ASCDE, Dispatch, and Market Value Modules}
}

## Related Resources
MISO Planning: MISO LOLE Study Reports

NREL ATB: Annual Technology Baseline

VALCOE: IEA Value-Adjusted LCOE Methodology

Contact & License

Maintainer: Justin Candler (Nous Enterprises LLC) Contact: Nousentllc@gmail.com License: MIT License – Free for academic and non-commercial use with attribution.
