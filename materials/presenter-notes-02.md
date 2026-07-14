# Presenter notes - Session 2 · Where data lives

## Preflight (5 min before)
- Open courses/02-where-data-lives.html, click Projector zoom to 125%.
- Test the sorter widget once (Apply-along 2): place one right, one wrong - confirm shake + green.
- Have your own "shadow spreadsheet" story ready (every presenter has one - name it).
- Whiteboard marker for the two-lane OLTP/OLAP drawing fallback.

## Run of show
- 0-3 · Welcome. Callback to Session 1 homework: "who ran the ladder test? what survived?" Two hands, 30 seconds each. Frame today: "last week WHAT data is, today WHERE it lives."
- 3-8 · Part 1 OLTP vs OLAP. Race car vs freight train metaphor first, jargon second. Land the Black Friday line: the CFO report and the checkout button fighting over the same engine. Amazon 2004 holiday story from the card, 60 seconds.
- 8-14 · Part 2 the city map. Walk the SVG left to right: shops, library, branches, harbor, merge. Netflix lakehouse story, then the swamp stat - pause after "80% became swamps". Land the exec question: "who owns the catalogue?"
- 14-18 · Part 3 pipelines. Follow order #4812 through the timestamps out loud - 00:00, 02:00, 08:00. Land "wrong, or just late?" as the week's takeaway phrase. Airbnb Airflow story only if time allows.
- 18-24 · Apply-along 1 map your company. Solo 2 min, then hunt the shadow spreadsheet together. Every room finds one within a minute - celebrate it as evidence, not shame.
- 24-32 · Apply-along 2 sorter widget. One volunteer drives on screen or everyone on devices. The live stock check causes the best argument - let it run 2 min, then name the rule: workload decides, not vocabulary.
- 32-39 · Apply-along 3 freshness audit. Quiet and personal - protect the writing minute. Harvest 2-3 "the question I will send my data engineer" lines.
- 39-45 · Q&A + quiz. Quiz solo on devices, then show of hands per question.

## Never cut
- The Black Friday two-lane story - it is the session's spine and the reason the whole map exists.
- "Who owns the catalogue?" - the one question that separates lakes from swamps.
- Apply-along 3 step 4 (the engineer question they will actually send) - the take-home behavior.

## Cut if long
- Row vs column storage detail - point at the self-study card ("the ledger intuition is on the page").
- The Airbnb Airflow story - point at the card instead.
- Apply-along 1 neighbor comparison - go straight from solo mapping to the shadow spreadsheet hunt.

## Expected questions
- "Which should WE buy: warehouse, lake or lakehouse?" - Wrong first question. Start from workloads and who owns governance; the architecture follows. Bring your map from Apply-along 1 to your data lead.
- "Why do we need copies of data everywhere - is that not wasteful?" - It is physics, not waste: two workloads need two engines. The waste is unGOVERNED copies - that is what the catalogue question checks.
- "Our dashboard numbers never match finance's - which store is lying?" - Usually neither: two pipelines with different cleaning rules. Session 4's metric layer is the fix; today's freshness audit finds the fork.
- "Is real-time data not always better?" - Real-time costs real money. Ask what decision changes at minute-level freshness vs nightly. For most board metrics, nightly is honest and cheap.
- "What is Kimball vs Inmon and should I care?" - Two classic warehouse design schools. Recognize the names, let your architects pick; your job is the catalogue and ownership questions.
