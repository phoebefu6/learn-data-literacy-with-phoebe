# Presenter notes - Session 7 · ML basics II: segment and understand customers

## Preflight (10 min before)
- Open `courses/07-ml-basics-segment.html`, projector zoom on, all cards collapsed.
- Run the KMEANS widget once and DEMO THE ASSIGN/MOVE ALTERNATION yourself - the room copies your rhythm. Confirm convergence lands in a handful of rounds and the three groups are visibly separable.
- Run the CLV widget once: check baseline reads ~3x, then rehearse both challenges (CAC to $150, lifespan 3 → 4) so you can narrate the verdict changes without hunting.
- Keep Session 5 (RFM grid) one tab away - Part 1 calls back to it explicitly.

## Minute-by-minute
- 0-3 · Welcome. Frame: "Session 6 predicted the future; today we understand the present." Boundary up front: recommendations, search and GenAI are out of scope - future AI literacy course.
- 3-8 · Part 1 unsupervised + k-means. Walk the four-panel SVG: drop pins, assign, move, repeat. Choosing k = judgment call; segments must be nameable and actionable or they are noise. Hierarchical = one line. RFM × clustering: rules give the grid, clustering finds shapes you did not look for. Tesco Clubcard story.
- 8-12 · Part 2 sentiment. Recipe: lexicon → bag-of-words + naive bayes. Pipeline SVG: 10,000 reviews → one product decision. Honest limit: sarcasm ("Great, delayed again"). Airline service-recovery story.
- 12-18 · Part 3 CLV. Workhorse formula SVG: AOV × frequency × margin × lifespan = $288 vs CAC $95 ≈ 3x. Historic vs predictive vs cohort middle. Name-drop BG/NBD + Gamma-Gamma. Harrah's mid-tier locals story - the room's favorite, do not rush it.
- 18-28 · Apply-along 1: kmeans widget. Everyone alternates assign/move until converged, then NAMES the three segments (bargain-occasional, frequent-regular, big-basket-rare) and writes one action each.
- 28-36 · Apply-along 2: clv widget. Baseline read, challenge 1 (CAC $150), challenge 2 (lifespan 4 years), compare end states out loud.
- 36-40 · Apply-along 3: segment reality check. Same-email test: if every segment gets the same email, you have zero real segments.
- 40-45 · Q&A + quiz.

## Never-cut beats
- THE ALGORITHM FINDS THE SHAPE; HUMANS NAME IT AND ACT. Say it at the kmeans debrief and again in closing - it is the whole story of applied ML.
- Segments must be nameable and actionable or they are noise.
- CLV:CAC under 1x = losing money on every customer you acquire; ~3x healthy.

## Cuts if long
- Hierarchical clustering one-liner - it is already just one line; drop it silently.
- Sentiment "exec move" tip (themes vs single score) - point at the page.
- Apply-along 3 becomes homework; keep the same-email test sentence in your close.

## Expected questions
- "Should we use AI to read our reviews instead?" → Boundary line: LLM-based text understanding is the AI literacy course. Basic sentiment is the honest 80% for triage - cheap, fast, explainable. Upgrade when sarcasm and nuance are actually costing you decisions.
- "How do we know k=3 is right?" → You do not, statistically - elbow hints, management decides. The real test: can you brief each segment in one sentence and fund a distinct action? If not, wrong k.
- "Is clustering better than our RFM rules?" → Not better - complementary. Rules encode what you already believe; clustering surfaces what you did not think to look for. Run both, argue about the differences.
- "Which CLV number should we trust?" → Start cohort-based historic - it is auditable. Move to BG/NBD-style predictive only when you have a DS team and a decision that needs it.
- "Our CLV:CAC is 6x - great, right?" → Maybe underinvesting: you could likely afford more growth. Check payback period and whether CAC stays sane at higher spend before celebrating.
