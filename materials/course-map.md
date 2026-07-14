# learn-data-literacy-with-phoebe - course map

Audience: **business stakeholders and executives** (decision-maker literacy: what to ask, when to trust, how to act - not how to build).
Format: 8 sessions x 45 min (3 welcome / ~15 concepts / ~22 apply-along with interactive widgets / 5 Q&A).
Case style: **per-session real cases** (public, well-documented company stories), plus small realistic numbers inside widgets.
Interactivity: no code. In-page widgets (assets/widgets.js): sorter, mean-median playground, KPI tree calculator, funnel simulator, RFM scorer, forecast fitting game, churn threshold slider, k-means stepper, CLV calculator.
Boundary by design: NO deep learning, NO recommendations/search, NO GenAI - those live in the future AI-literacy course (teaser on Session 8 + index).

## Session map

| # | Title | Diff | Anchor real case | Core content | Widget(s) |
|---|-------|------|------------------|--------------|-----------|
| 1 | Think in data | 🟢 | Oakland A's (Moneyball); Target's pregnancy score cautionary tale | Data types (structured/semi/unstructured; nominal/ordinal/interval/ratio); Data -> Information -> Insight -> Action ladder + "so what?" test; analytics project lifecycle (CRISP-DM in plain language); DA/DE/DS/BI roles | sorter (classify statements onto the ladder) |
| 2 | Where data lives | 🟢 | Journey of one Amazon order; Netflix lakehouse | Application DB; OLTP vs OLAP (row vs column); warehouse vs mart vs lake vs lakehouse ("city map"); ETL vs ELT; what to ask your data engineer | sorter (scenario -> right store) |
| 3 | EDA and stats that do not lie | 🟡 | Bing's $100M title experiment (Kohavi); UC Berkeley admissions (Simpson's paradox) | Descriptive stats (mean/median/mode, spread, percentiles); distributions and outliers; why averages lie; EDA workflow; correlation vs causation; sampling; A/B intuition; chart-choice cheat sheet | meanmedian (whale-client outlier playground) |
| 4 | Metrics and KPI trees | 🟡 | Amazon flywheel + WBR metrics culture; North Star examples (Airbnb nights booked, Spotify time listening) | Drucker: what is not measured cannot be improved; good metric criteria; vanity vs actionable; North Star + inputs + guardrails; KPI decomposition: income = revenue - cost; revenue = buyers x basket size x basket value; buyers = new + returning + resurrected - churned; diagnosing "revenue down 8%" via the tree | kpitree (live P&L tree calculator) |
| 5 | Funnels, cohorts and RFM | 🟡 | Dropbox referral (AARRR); Baymard ~70% cart abandonment; Facebook "7 friends in 10 days"; Sephora/Starbucks loyalty (RFM) | Funnel analytics (conversion, drop-off, fix-here-first); AARRR; cohort analysis + retention curves; RFM scoring + segment grid + action per segment; industry metric packs: Internet (DAU/MAU, stickiness), SaaS (MRR/ARR, NRR, churn, CAC, LTV, CAC payback), E-com (GMV, AOV, conversion, repeat rate) | funnel (simulator) + rfm (scorer) |
| 6 | ML basics I: predict numbers and labels | 🟠 | Walmart demand forecasting; telco churn (the classic churn problem) | Supervised learning intuition; train/test; overfitting in one picture; sales forecasting: regression + time-series intuition (trend/seasonality, moving average, ARIMA/Prophet as names); churn prediction: logistic regression, decision tree, random forest + gradient boosting (XGBoost/LightGBM as names); evaluation literacy: MAPE/RMSE, precision vs recall, why accuracy lies on imbalanced data | forecast (fit trend+seasonality, beat the gut) + threshold (precision/recall slider) |
| 7 | ML basics II: segment and understand customers | 🟠 | Tesco Clubcard / dunnhumby (segmentation); airline Twitter sentiment; Harrah's casino (CLV) | Unsupervised intuition; k-means (+ hierarchical dendrogram idea); choosing k; RFM x clustering -> personas -> action; sentiment analysis basics (lexicon -> bag-of-words + naive bayes); CLV: historic vs predictive, cohort CLV, BG/NBD + Gamma-Gamma as names; CLV:CAC decisions; product analytics (activation, adoption, paths) | kmeans (stepper) + clv (calculator) |
| 8 | From dashboard to decision | 🔴 | Amazon Weekly Business Review discipline; Domino's data-driven turnaround framing | Full loop on one worked mini-case: KPI tree diagnosis -> funnel -> cohort -> RFM segments -> forecast -> action memo; insight-to-action memo template (answer first); metric review meeting hygiene; honest boundary: deep learning, recsys, search, GenAI -> AI literacy course | kpitree + funnel reused with case numbers |

## Model list (all at executive-intuition level)

| Model | Session | Business use taught | Depth |
|---|---|---|---|
| Linear regression | 6 | Sales forecasting, driver analysis | intuition + read-the-output |
| Moving average / trend + seasonality / ARIMA / Prophet | 6 | Demand forecasting | names + decomposition intuition |
| Logistic regression | 6 | Churn / conversion propensity | intuition |
| Decision tree | 6 | Explainable churn rules | intuition |
| Random forest / gradient boosting (XGBoost, LightGBM) | 6 | "Names to recognize" tier | name-drop + when they win |
| k-means | 7 | Customer segmentation | stepper widget intuition |
| Hierarchical clustering | 7 | Dendrogram idea | mention |
| Naive bayes on bag-of-words | 7 | Sentiment on reviews | intuition |
| RFM (rule-based) | 5, 7 | Segmentation baseline | full working method |
| Cohort CLV; BG/NBD + Gamma-Gamma | 7 | Customer lifetime value | cohort method working; BG/NBD name-drop |

## Framework list

DIKW ladder (data-information-insight-action) · CRISP-DM lifecycle · OLTP/OLAP + warehouse/lake/mart/lakehouse · Tukey EDA · A/B testing (Kohavi) · Drucker measurement principle · North Star framework · KPI decomposition trees · growth accounting (new/returning/resurrected/churned) · AARRR (McClure) · funnel analytics · cohort retention · RFM (Hughes) · SaaS metric stack · e-com metric stack · DAU/MAU stickiness · CLV:CAC (3x rule) · confusion-matrix literacy · answer-first memo (Minto, cross-link to strategic thinking course)

## Canon / sources credited on pages

Provost & Fawcett *Data Science for Business* · Croll & Yoskovitz *Lean Analytics* · Kohavi et al *Trustworthy Online Controlled Experiments* · Barbara Minto *Pyramid Principle* · Arthur Hughes RFM · Fader & Hardie CLV papers · Kimball vs Inmon warehouse schools · Davenport *Competing on Analytics*

## Not covered by design

Deep learning, neural networks, embeddings, recommendations, search ranking, GenAI/LLMs (future learn-ai-literacy course) · SQL/Python syntax (this is literacy, not tooling) · statistics math proofs · MLOps/deployment · data privacy law depth (one guardrail card only)
