<!-- phoebe header -->

[![Open the live course](https://img.shields.io/badge/%E2%96%B6%20open%20the%20live%20course-1f6feb?style=for-the-badge)](https://phoebefu6.github.io/learn-data-literacy-with-phoebe/)
[![Star this repo](https://img.shields.io/github/stars/phoebefu6/learn-data-literacy-with-phoebe?style=for-the-badge&label=star%20this%20repo&color=444444)](https://github.com/phoebefu6/learn-data-literacy-with-phoebe/stargazers)
[![Free courses](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fphoebefu6.github.io%2Flearn-with-phoebe%2Fstats.json&query=%24.courses_live&label=free%20courses&style=for-the-badge&color=111111)](https://phoebefu6.github.io/learn-with-phoebe/)

### ▶︎ [Open the live course →](https://phoebefu6.github.io/learn-data-literacy-with-phoebe/)

Free, runs in your browser. No install, no login.

> 📚 Part of **[Learn with Phoebe](https://phoebefu6.github.io/learn-with-phoebe/)** - free, hands-on courses on AI, data, and the craft around them. **[Browse every course ↗](https://phoebefu6.github.io/learn-with-phoebe/)**

<!-- /phoebe header -->

# learn-data-literacy-with-phoebe

Data literacy for business stakeholders and executives - from numbers to decisions. Eight 45-minute sessions that teach decision-makers what to ask, when to trust, and how to act on data: metrics and KPI trees, funnels, cohorts and RFM, forecasting and churn intuition, and the insight-to-action memo. Every session anchors on a real company case (Moneyball, Amazon, Netflix, Tesco, Bing) and an in-page interactive simulator - sliders, not syntax. No code anywhere.

## Sessions

| # | Title | What you learn | Widget |
|---|-------|----------------|--------|
| 1 | Think in data | Data types, the data-to-action ladder, the analytics lifecycle | Ladder sorter |
| 2 | Where data lives | OLTP vs OLAP, warehouse / mart / lake / lakehouse, ETL vs ELT | Data-store sorter |
| 3 | EDA and stats that do not lie | Why averages lie, outliers, correlation vs causation, A/B intuition | Mean-median playground |
| 4 | Metrics and KPI trees | North Star metrics, vanity vs actionable, KPI decomposition | Live P&L tree calculator |
| 5 | Funnels, cohorts and RFM | Funnel drop-offs, AARRR, retention curves, RFM segments, metric packs | Funnel simulator + RFM scorer |
| 6 | ML basics I: predict | Forecasting, churn prediction, precision vs recall literacy | Forecast game + threshold slider |
| 7 | ML basics II: segment | k-means personas, sentiment basics, customer lifetime value | k-means stepper + CLV calculator |
| 8 | From dashboard to decision | Full capstone case, the answer-first memo, weekly metric review | KPI tree + funnel reused |

## Run locally

```
cd learn-data-literacy-with-phoebe
python3 -m http.server 8000
```

Then open http://localhost:8000 in a browser.

## Structure

```
learn-data-literacy-with-phoebe/
  index.html            landing page with paths and difficulty legend
  assets/               style.css, app.js, widgets.js (all 9 simulators)
  courses/              01-think-in-data.html ... 08-dashboard-to-decision.html
  materials/            course-map.md, presenter notes
```

by Phoebe Fu

Sibling courses: [learn strategic thinking](https://phoebefu6.github.io/learn-strategic-thinking-with-phoebe/) · [learn claude](https://phoebefu6.github.io/learn-claude-with-phoebe/) · [learn codex](https://phoebefu6.github.io/learn-codex-with-phoebe/) · [learn markdown](https://phoebefu6.github.io/learn-markdown-with-phoebe/) · [learn mermaid](https://phoebefu6.github.io/learn-mermaid-with-phoebe/) · [learn html](https://phoebefu6.github.io/learn-html-with-phoebe/)
