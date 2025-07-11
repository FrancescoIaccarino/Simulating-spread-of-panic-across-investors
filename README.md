# Investor Fear Goes Viral – Modeling Panic in TSLA During COVID-19

This project explores the contagion of investor sentiment using epidemiological models applied to Tesla (TSLA) stock in early 2020. By treating fear as a transmissible phenomenon, we simulate how panic spread among investors during the COVID-19 outbreak using SIR, SIS, SIRS, and SEIR frameworks.

> MSc in Data Science & Business Analytics @ Bocconi University

---

## 🔍 Overview

We developed a bespoke Fear Sentiment Index (FSI) from financial news and social media posts about TSLA, which serves as our proxy for "infected" investors. We then fitted four epidemic models to this index to analyze how fear emerged, peaked, and dissipated.

## 🧪 Methodology

- **FSI Construction**: Textual analysis of TSLA-related content to derive a daily fear index.
- **Epidemic Models**:
  - `SIR`: One-wave panic, self-limiting contagion.
  - `SIS`: Persistent fear without lasting immunity.
  - `SIRS`: Temporary immunity leading to multiple fear waves.
  - `SEIR`: Exposed phase models delayed reaction to news.

- **Model Calibration**: Non-linear least squares on FSI curves.
- **Validation**: Sub-period fitting and comparison to historical market panic patterns.

## 📊 Key Insights

- The **SEIR model** best matched the TSLA fear trajectory.
- Early March 2020 represented the panic peak — ~35% of investors fearful.
- Aftershocks of fear occurred due to waning memory (SIRS).
- Network models did not improve results significantly, suggesting global news led to near-complete investor connectivity.

## 💡 Implications

- Circuit breakers can serve as effective "social distancing" in markets.
- Investor sentiment peaks are detectable with structured contagion modeling.
- Early intervention during "exposed" sentiment phases may prevent full-blown panic.
