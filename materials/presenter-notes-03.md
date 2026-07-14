# Presenter notes - Session 3 · EDA and stats that do not lie

## Preflight (5 min before)
- Open courses/03-eda-and-stats.html, click Projector zoom to 125%.
- Test the meanmedian widget once (Apply-along 1): click "Add the whale client", confirm the mean jumps and the median barely moves, then reset.
- Bring one real anonymized slide with an "average" claim for Apply-along 2 (in case the room has none handy).
- Whiteboard marker for the skewed-distribution sketch fallback.

## Run of show
- 0-3 · Welcome. Callback: "who asked 'what is the median?' is a Session 3 spoiler - who asked their data engineer the freshness question?" Frame today: "how numbers lie politely, and the four questions that stop them."
- 3-8 · Part 1 describe before you decide. Mean/median/mode fast, then park on spread: same average, different business. Census income gap story, 45 seconds. Land the exec move: "what is the median?"
- 8-12 · Part 2 EDA. Tukey's detective framing, then walk the chart-choice table row by row - the "no pie beyond 4 slices" line always gets a laugh and always sticks. Tease Anscombe as homework: "four identical stat sheets, four different truths - the card has it."
- 12-18 · Part 3 correlation, causation, paradox. Ice cream and drownings first (60 seconds, gets the concept for free). Then Berkeley on the SVG - point at the two rising groups and the falling blend. Close with Bing $100M plus the honesty beat: most tested ideas fail.
- 18-25 · Apply-along 1 meanmedian widget. Predictions OUT LOUD before anyone clicks - the gasp when the mean jumps is the whole lesson. Then the board-pack debate: median plus whale named separately.
- 25-33 · Apply-along 2 stat-proof one slide. Solo rewrite 4 min, protect the writing time. Harvest 2 before/after pairs - read both versions aloud, let the gap speak.
- 33-39 · Apply-along 3 correlation courtroom. Run all 4 claims at pace, vote by hands, one confounder each. Claim 3 (support contact) lands hardest - do not rush its debrief.
- 39-45 · Q&A + quiz. Quiz solo on devices, then show of hands per question.

## Never cut
- The whale widget prediction moment - predicting before clicking is what makes the lesson stick.
- The Berkeley reversal - it is the course's single most repeated story in later sessions.
- "Most A/B ideas fail" - without the honesty beat, the Bing story teaches overconfidence instead of testing.

## Cut if long
- Percentiles depth - point at the self-study card ("p90 grammar is on the page").
- Correlation courtroom claims 2 and 4 - run 1 and 3 only.
- The Wald bombers sampling story - point at the card instead.

## Expected questions
- "So should we never use the mean?" - Use both. Mean answers "total per head", median answers "typical". The gap between them is itself a finding: it means whales.
- "How many data points is enough?" - No universal number; the honest move is showing n on every slide. Your analysts own the significance math; you own asking for n.
- "Can we A/B test everything?" - No: some things are too slow, too rare or unethical to randomize. Reserve experiments for big reversible bets; elsewhere, confounder discipline plus judgment.
- "What about statistical significance and p-values?" - Deliberately left with your analysts. Your literacy job: baseline, center, n, confounder. If a claim passes those four, THEN ask them about significance.
- "Our sample is all customers, not a sample - does sampling still matter?" - Yes: your customers are a sample of the market, survivors of your churn. The Wald question still applies - who is missing?
