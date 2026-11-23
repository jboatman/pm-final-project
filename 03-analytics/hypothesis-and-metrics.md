# Hypothesis & Success Metrics (Module 3)

## Pre-work · Hypothesis check
- **Role , who you are solving for (from M2):** The Discerning Curator/Seeker: a film-literate viewer who judges StreamLine by the quality of its picks, not the size of its catalog.
- **Goal , what this user is ultimately trying to achieve:** To find a film that fits their taste, recommended by a source they trust, without scrolling through a sea of titles.
- **Friction / moment of misery , the specific pain blocking their goal:** Recommendations and search miss their taste. "Because you watched" serves more sequels, and "slow quiet French drama" returns Fast & Furious. They scroll, give up, or leave.
- **Current workaround , the external tool or manual process they rely on (M2):** They get picks outside the app, from friends or a competitor's weekly hand picked email, then search StreamLine for the exact title. Some cancel and switch to the competitor.
- **Problem Hook , your one-sentence framing of the business crisis (M1):** We must stop StreamLine's slide into a commoditized, mid content warehouse by fixing the endless, low trust browsing that leaves viewers scrolling, rewatching, or leaving for competitors that hand-pick for them.
- **Value Proposition , the outcome your initiative promised to deliver (M1):** Spotlight replaces the 15,000 title scroll with three picks a night, each labeled with a trusted source (a critic, our editors, or viewers like them) and matched to the viewer's chosen lens, so viewers choose faster and choose better.

## Read your data snapshots
- **Does the funnel data confirm your M2 friction point, or does it tell a different story? Note where the numbers align with the qualitative pain you found and where they diverge.:** Mostly confirms, with one twist. 71% of visitors browse but only 29% start playing, which matches the M2 pain of giving up before choosing. "Searched then played" also fell from 41% to 34%, consistent with search failing. The twist: only 11% reach 30 minutes, so about 62% of plays end early. That could be bugs (playback, resume) or poor matches, so I'll fix the bugs first, then re-check the drop.
- **Do the retention patterns align with the workaround your M2 persona used to find content? Note what the Mo. 0→1 drop suggests about the onboarding experience your persona described as frustrating.:** Yes, it aligns. My persona leaves the app to get trusted picks from friends or a competitor's email. Spotlight cohorts, which get picks in the app, retain 11–15 points better at Month 1 (74–79% vs. 63–68%) and 13–18 points better at Month 3. Retention also improves with each new Spotlight cohort, while it falls with each Full Library cohort. The Mo. 0 to 1 drop (21–26% even with Spotlight) suggests new subscribers still hit the scroll before they trust anything. That points to the first week experience: they need good picks right away, which is the job of our setup stage.
- **Does the LTV gap and the content mix (61% trending for Wanderers) confirm the moment of misery your persona described? Note which segment your persona is in and whether the data confirms their pain.:** It confirms the pain, but in a different segment than my persona. My Discerning Curator Seeker looks most like a Power User: they already find curated content (58% curated), use the app most, and rarely churn, so they aren't the biggest opportunity. The pain I described (scrolling, giving up, defaulting to whatever's popular) shows up most in Wanderers: 61% trending, 1.1 sessions a week, lowest LTV. That matches my secondary persona, the Overwhelmed Evening Viewer (Priya, Aisha, the focus group). Wanderers are also 41% of the base and show the biggest churn drop with Spotlight (22 pts). Pivot: make the Overwhelmed Evening Viewer the primary persona and keep the Curator Seeker as the design inspiration.
- **Does the low adoption confirm your persona is burdened by tools they don’t use? Note whether the low scheduling adoption (42%) for coordinators matches your M2 moment of misery.:** _(not filled in)_
- **Does the workflow data match the manual process or hack you documented in M2? Note whether the specific drop-offs or time gaps explain why your persona avoids the digital tool.:** _(not filled in)_
- **Look at the CSAT heatmap. Which specific cell most directly maps to your persona’s friction? Note how the NPS trend justifies the urgency of your M1 Problem Hook.:** _(not filled in)_

## Step 3 · Craft your hypothesis
- **Qualitative evidence (from M2) , quote the specific friction / moment of misery for your persona:** "I open the app, scroll for like twenty minutes, and close it without watching anything. There's 15,000 titles but nothing I actually want." (Priya, UXR-01). The focus group adds: they'd rather someone "just tell me what's good tonight" (UXR-12).
- **Quantitative evidence (from M3) , name the metric or data point that confirms the pain; cite the number:** Wanderers are 41% of subscribers, with the lowest LTV ($8.40), 1.1 sessions a week and 61% trending content. Their churn is 22 pts lower when exposed to Spotlight. Across all users, 71% browse but only 29% start playing.
- **Persona , role, goal, and the friction you confirmed in the reconciliation steps:** The Overwhelmed Evening Viewer ("Wanderers"). They open the app to unwind and want something good tonight in minutes. Instead they scroll, give up, or default to whatever's trending.
- **Problem you are solving , one sentence describing the specific friction this initiative removes:** Spotlight replaces the 15,000 title scroll with three trusted, labeled picks a night, so Wanderers stop giving up before they find something worth watching.
- **Strategic outcome , what behaviour change do you expect, and how does it map to retention / revenue / churn?:** Wanderers choose faster and finish what they start, so they come back more often. More sessions lower churn and lift LTV from $8.40 toward the Casual Browser level ($11.40).
- **Primary success metric (initiative signal) , the leading indicator that tells you the gap is closing:** 7 day completion rate of started titles among Wanderers, target +15% vs. control. Time to first play is the earliest read.
- **Guardrail metric (product signal) , the metric that must NOT drop; it protects your existing base:** Weekly watch time and churn for Power Users must not drop. They're the highest LTV segment (22% of subscribers, $14.20), and Spotlight changes the home screen they already use well.
- **Decision window , how much time or data before you scale, pivot, or kill? minimum threshold to proceed?:** A 6-week A/B test, started after the Phase 0 bug fixes ship.
Scale at +15% or more with no guardrail drop.
Iterate at +5% to 15%.
Kill below +5% or if Power User watch time drops.
- **Draft your full hypothesis sentence , one to three sentences; quote the metric, name the persona, name the outcome:** Based on Priya's 20 minute scroll that ends in nothing watched and data showing Wanderers (41% of subscribers) churn 22 pts less when exposed to Spotlight, I believe that replacing the scroll with three trusted, labeled picks a night for Overwhelmed Evening Viewers will result in them choosing faster and finishing what they start, as measured by a 15% increase in 7 day completion rate. I will protect Power User watch time and churn and will make a go/no go decision after a 6 week A/B test.

---

## Success metrics summary

| Metric | Type | Target | Why it matters |
|---|---|---|---|
| 7-day completion rate of started titles (Wanderers) | Primary / north star | +15% vs. control | Shows picks were good, not just appealing |
| Time to first play (median, autoplay excluded) | Leading | Faster than control | Shows choosing got easier |
| Early abandonment (stopped in <10% of runtime) | Diagnostic | No rise | Catches picks that look appealing but disappoint |
| Power User weekly watch time and churn | Guardrail | No drop | Protects the highest-LTV segment (22%, $14.20) |

_15% and 6 weeks are placeholders. Thresholds: scale at +15% or more with no guardrail drop, iterate at +5–15%, kill below +5%._

## Working notes

_Reasoning behind the answers above, kept for future discussion._

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
