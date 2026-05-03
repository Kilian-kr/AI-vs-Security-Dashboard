# 🛡️ AI & Cybersecurity Impact Dashboard

> **Status: 🚧 Work in Progress**  
> This Power BI dashboard is currently under active development.

---

## Overview

This dashboard investigates whether the rise of AI adoption has had a measurable effect on the cybersecurity landscape. It combines publicly available data on AI usage across companies and developers with threat intelligence data on CVEs, phishing attacks, and security incidents — tracking trends from 2021 to 2025.

The goal is to surface correlations (or the absence thereof) between increasing AI adoption and shifts in the volume and severity of cyber threats.

---

## Screenshots

### Executive Overview
![Executive Overview](https://github.com/Kilian-kr/AI-vs-Security---Dashboard/blob/main/screenshots/screenshot_executive_overview.png?raw=true)

### Cyber Security Deep Dive
![Cyber Security](https://github.com/Kilian-kr/AI-vs-Security---Dashboard/blob/main/screenshots/screenshot_cyber_security.png?raw=true)

---

## Dashboard Pages

### 1. Executive Overview
A high-level summary page presenting the most important KPIs side-by-side across two domains:

**Cyber Security**
- Total CVEs Published 
- Phishing Attacks Reported 
- Security Incidents 

**AI Adoption**
- Global AI Adoption Rate

Includes a dual-axis combo chart showing monthly CVE publications and phishing attacks across 2025.

---

### 2. Cyber Security Deep Dive
A detailed trend analysis page anchored to a baseline of January 1, 2021:

**Baseline values (01.01.2021)**
- 742 CVEs Published
- 246K Phishing Attacks
- 53 Security Incidents

Includes:
- **Indexed Trend Chart (2021–2025):** Tracks CVEs, phishing attacks, and security incidents relative to the 2021 baseline (Index = 100 × Actual / Baseline)
- **Year-over-Year Change Chart:** Area chart showing annual percentage change per metric from 2022 to 2025

---

## Research Question

> **Has increasing AI adoption influenced the frequency or nature of cybersecurity threats?**

Hypotheses being explored:
- AI tooling lowers the barrier for attackers → increase in phishing/CVEs
- AI-assisted defenses reduce incident rates → decrease in security incidents
- No statistically significant correlation exists between AI adoption rates and threat volumes

---

## Data Sources

| Dataset | Source | Update Frequency |
|---|---|---|
| AI Adoption – Companies | [Our World in Data](https://ourworldindata.org/grapher/share-companies-using-artificial-intelligence) | Annual |
| AI Adoption – Developers | [Stack Overflow Developer Survey](https://survey.stackoverflow.co/) | Annual |
| CVEs Published | [NIST NVD JSON Data Feeds](https://nvd.nist.gov/vuln/data-feeds#divJson20Feeds) | Continuous |
| Phishing Attacks | [PhishTank](http://data.phishtank.com/data/online-valid.csv) | Daily |
| Security Incidents | [EuRepoC](https://eurepoc.eu/de/detaillierte-tabellenansicht/) | Ongoing |


---

## Known Limitations & Open Issues

- [ ] Phishing data from PhishTank may undercount attacks (only verified/reported URLs)
- [ ] EuRepoC covers primarily European and state-sponsored incidents — not a global sample
- [ ] AI adoption survey data (Stack Overflow) reflects developer sentiment, not enterprise reality
- [ ] Correlation analysis methodology not yet finalized
- [ ] AI Adoption section on Executive Overview currently shows only global rate — developer-specific breakdown pending

---

## Roadmap

- [ ] Add developer AI usage breakdown from Stack Overflow (by tool, by year)
- [ ] Add AI Adoption detail page (mirroring Cyber Security deep dive)
- [ ] Implement correlation analysis visual 

---


> Requires **Power BI Desktop** (free) — download at [powerbi.microsoft.com](https://powerbi.microsoft.com/desktop/)

---

## Contributing

This dashboard is currently a solo project. If you spot data quality issues or have suggestions for additional sources, feel free to open an issue.

---

*Last updated: May 2026*