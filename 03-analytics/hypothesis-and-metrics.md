# Hypothesis & Success Metrics

> **Module 3 · ★ Deliverable 3.** Repo file `03-analytics/hypothesis-and-metrics.md` — part of your submission.
> Do the lab in the **Module 3 · Exercise Guide** (linked from the Module 3 deck), then click **⬇ Download .md** — it saves as this exact file. Commit it here.
> It feeds the **Problem, Value & Hypothesis** slide of your Module 6 final deck.

## Finalized product hypothesis

> Based on [qual + quant evidence], I believe that [solving X] for [persona] will result in [outcome], as measured by a [X%] change in [success metric]. I will protect [guardrail metric] and make a go/no-go decision after [decision window].

## Success metrics

| Metric | Type | Target | Why it matters |
|---|---|---|---|
| _North-star_ | | _____ | _____ |
| _Leading indicator_ | | _____ | _____ |
| _Guardrail_ | | _____ | _____ |

---

## Working notes (before the lab export)

_Keep these when replacing this file with the guide's export._

### Decision: fix bugs first, then re-read the depth drop

**Added:** 2026-11-23 · **Status:** Open · **Revisit:** after Phase 0 ships

Snapshot 1 (Engagement & Funnel Health) shows 29% of visitors start playing but only 11% reach a 30-minute session, so **about 62% of plays end early**. We can't yet tell why:

| Possible cause | Evidence today | What it would mean |
|---|---|---|
| **Bugs** cut sessions short | Playback failures (BUG-1042), resume restarting at 0:00 (BUG-1061), watchlist not syncing (BUG-1058) | A fix problem, not a curation problem |
| **Poor match:** viewers start titles that don't hold them | Comfort rewatches (Aisha, UXR-03), sequel loop (Marcus, UXR-02; BUG-1091) | Spotlight's "choose better" case, measured by completion |

**Plan**
1. **Ship the Phase 0 bug fixes first** (BUG-1042, BUG-1058, BUG-1061), as already planned.
2. **Re-pull the start → 30-minute drop** a few weeks after the fixes ship and compare it with today's 62%.
3. **Decide what the drop means:**
   - **It recovers a lot:** bugs were the main cause. Spotlight's case rests on *choosing* (browse → play), and time to first play matters more.
   - **It barely moves:** the poor match is real. 7-day completion stays the primary success metric.
   - **In between:** both causes are real. Size the bug share before setting the completion target.

**Check we can run now:** split early-abandoned plays into sessions that hit a playback error or resume restart and sessions that didn't. If most early exits have no bug, poor match is already the likelier cause.

**Why it matters:** if we launch Spotlight before the fixes, any completion lift (or lack of one) is mixed up with bug effects, and the A/B test can't tell us whether the curation works.

### Snapshot 2: retention cohorts (Spotlight vs. Full Library)

**Added:** 2026-11-23 · **Status:** Open

**What the data shows**
- Spotlight cohorts (Dec–Feb) retain **11–15 pts better at Month 1** (74–79% vs. 63–68%) and **13–18 pts better at Month 3** (52% vs. 34–39%).
- Each new Spotlight cohort retains better than the last (74% → 77% → 79% at Month 1), while each new Full Library cohort retains worse (68% → 66% → 63%).
- The **Month 0 → 1 drop is still the largest leak**: 21–26% with Spotlight, 32–37% without.

**Notes for future discussions**
1. **Correlation, not proof.** The cohorts started in different months, and holiday sign-ups (Dec, Jan) may behave differently from fall ones. Seasonality or other changes could explain part of the gap. **We still need an A/B test**, which supports the Module 3 and 5 plan.
2. **This supports Stage 0 (setup).** The biggest leak is the first month, before Spotlight has learned anything about the viewer. New subscribers still hit the scroll before they trust anything, so the first-week experience (setup plus strong first picks) is where to focus.
3. **Bugs may feed the Month 0 → 1 drop too.** Losing saved titles in the first weeks (BUG-1058) could push new subscribers out. This is the same bugs-first logic as the Snapshot 1 note: re-check this drop after Phase 0 ships.

### Snapshot 3: segments, and the persona pivot

**Added:** 2026-11-23 · **Status:** Decided

| Segment | % of base | Monthly LTV | Sessions/wk | Content mix | Churn with Spotlight |
|---|---|---|---|---|---|
| Power Users | 22% | $14.20 | 4.8× | 58% curated / 22% trending | N/A (low churn anyway) |
| Casual Browsers | 37% | $11.40 | 2.3× | 31% curated / 44% trending | −14 pts |
| **Wanderers** | **41%** | **$8.40** | **1.1×** | **18% curated / 61% trending** | **−22 pts** |

**Decision: make the Overwhelmed Evening Viewer the primary persona.**
- **The Curator-Seeker looks like a Power User.** They already find curated content, use the app most and rarely churn, so they're not the biggest opportunity (the pivot check).
- **The pain shows up in Wanderers.** Scrolling, giving up and defaulting to whatever's trending matches the Overwhelmed Evening Viewer (Priya UXR-01, Aisha UXR-03, focus group UXR-12).
- **They're the largest segment with the biggest response.** 41% of the base and a 22-pt churn drop with Spotlight.
- **The strategy carries over.** "Easy tonight" becomes the default lens; the Curator-Seeker stays as design inspiration and the Hidden gems lens.
- **Caveat:** "churn if Spotlight-exposed" compares exposed vs. non-exposed users, who may differ in other ways. The A/B test still has to confirm it.

### Draft hypothesis (updated for the pivot)

> Based on 7 of 12 research sessions showing viewers giving up or distrusting recommendations, and Snapshot 3 showing Wanderers (41% of subscribers) churn 22 pts less when exposed to Spotlight, we believe that replacing the scroll with three source-labeled Spotlight picks for **Overwhelmed Evening Viewers (Wanderers)** will result in viewers choosing faster and choosing better, as measured by a **15% increase in 7-day completion rate** of started titles. We will protect **weekly watch time per subscriber** and make a go/no-go decision after a **6-week A/B test**, run after the Phase 0 bug fixes ship.

_15% and 6 weeks are placeholders. Verify the "7 of 12" count against the sample data._
