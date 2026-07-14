# Presenter notes - Session 6 · ML basics I: predict numbers and labels

## Preflight (10 min before)
- Open `courses/06-ml-basics-predict.html`, click "Projector zoom: on", collapse all cards.
- Run the FORECAST widget once: slide trend, then seasonality, confirm MAPE updates and you can get under 6%.
- Run the THRESHOLD widget once: drag the slider both directions, confirm the flagged counts and red dots read clearly on the projector.
- Have Session 3 (stats) and Session 4 (metrics) tab-ready for callbacks.

## Minute-by-minute
- 0-3 · Welcome. Frame: "You will never train a model. You will judge one - harder job." State the boundary early: no deep learning, no GenAI, that is the AI literacy course.
- 3-8 · Part 1 supervised learning. Numbers vs labels, train/test as the unseen exam. Land the overfitting SVG: wiggly line = memorized the textbook. Plant the exec question: "how does it score on data it has never seen?"
- 8-13 · Part 2 forecasting. Sandwich: level + trend + seasonality + accepted noise. Moving average as the humble baseline every fancy model must beat. Walmart story: bad forecast = empty shelves or landfill. MAPE = average % miss.
- 13-19 · Part 3 classification. Churn as the canonical case. Walk the model ladder SVG left to right: logistic (auditable) → tree (readable) → forest/boosting (accurate, opaque). Then the accuracy trap: 5% churn, "nobody churns" = 95% accurate. Precision vs recall via the four-cell scorecard.
- 19-28 · Apply-along 1: forecast widget. Everyone slides trend first, then seasonality, race to MAPE under 6%. Debrief: you just did what Prophet does; the leftover wiggle is noise - chasing it is overfitting.
- 28-37 · Apply-along 2: threshold widget. Slide low (count wasted offers), slide high (count walkers), then pick YOUR threshold given a 20% discount per save call. Poll 3 people for their threshold - celebrate that they differ.
- 37-41 · Apply-along 3: spec one prediction. Label definition, training history, cost of each miss direction. This spec is the session's take-home deliverable.
- 41-45 · Q&A + quiz. Run the 3 questions live if time allows; homework otherwise.

## Never-cut beats
- THE THRESHOLD DECISION BELONGS TO THE BUSINESS. The model gives scores; the threshold prices false alarms against lost customers. If this is the only sentence they remember, the session paid for itself.
- The overfitting exam metaphor + the one exec question ("score on unseen data?").
- Accuracy lies on rare events - the 95%/5% churn trap.

## Cuts if long
- Part 2's "exec move" tip (baseline MAPE comparison) - point to the page instead.
- Apply-along 3 becomes pure homework (announce it, skip the room time).
- Self-study card "the data is the model" - never present it live anyway, just point.

## Expected questions
- "Should we just use AI for this?" → Boundary line: deep learning and GenAI are a different course. For tabular business data (churn, demand), THESE classic tools are still what wins in practice - boring, cheap, auditable.
- "Which model should my team pick?" → Wrong first question. Right one: what explainability does the decision require? Regulated or contested decisions walk you down the ladder; pure accuracy plays walk you up.
- "What is a good MAPE?" → Depends on the series - compare against the naive baseline, not an industry myth. The gap between model MAPE and baseline MAPE is what the modeling is worth.
- "Our vendor claims 98% accuracy." → Ask base rate first, then precision/recall on held-out data. Impossible-looking accuracy usually means a leaky label (the answer snuck into the features).
- "Can the model set the threshold itself?" → It can optimize a statistic, but it cannot know your margin, save-desk capacity, or brand cost of a false alarm. That is a business meeting, revisited quarterly.
