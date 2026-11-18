# Problem Hook & Value Proposition: StreamLine Spotlight

> **Module 1 · ★ Deliverable 1.** Repo file `01-product-thinking/problem-hook.md` — part of your submission.
> Do the lab in the **Module 1 · Exercise 2 Guide** (linked from the Module 1 deck), then click **⬇ Download .md** — it saves as this exact file. Commit it here.
> It becomes the **Problem, Value & Hypothesis** slide of your Module 6 final deck. (Your Module 1 · Exercise 1 discovery map lands in `strategic-map.md`.)

## 1. Chosen scenario

**Path:** StreamLine Spotlight (B2C)

A big catalog with flat engagement is a clear, relatable discovery problem, where curation can win back quality-focused viewers.

## 2. The strategic crisis

_The big-picture business risk. If the company does nothing for 12 months, what happens to its market position?_

> If we do nothing for 12 months, the company will be locked into the "warehouse of mid-tier content" label. Engagement will slide from a plateau into decline as quality-focused viewers move to curation-led rivals, leaving us competing on catalog size and price, a race we lose to bigger libraries.

## 3. The moment of misery

_The specific point where the product fails the user, forcing a manual workaround (Google, spreadsheets, group texts, a competitor)._

> The user is currently forced to give up or go elsewhere: after 20 minutes of look-alike tiles they close the app without watching (Priya went back to a DVD), rewatch the same few comfort shows (Aisha), trust friends over the algorithm (Sam), or cancel for a competitor that emails them hand-picked films (Tom).

## 4. Problem hook

_One urgent sentence fusing the business risk and the user pain, your pitch for why this is the most important thing to work on right now._

> We must stop StreamLine's slide into a commoditized, mid-tier content warehouse by fixing the endless, low-trust browsing that leaves viewers scrolling for 20 minutes, falling back on comfort rewatches, or leaving for competitors that hand-pick for them.

## 5. Value proposition

_Who it's for, the new value, and why it's urgent to launch now._

> For **discerning viewers who value quality over volume** (and the overwhelmed evening viewers who share the same pain), we will **replace the 15,000-title scroll with Spotlight: three standout picks a night from an editor-curated pool, matched to each viewer's taste and explained ("why this, why now"), in the app for subscribers and by weekly email for lapsed ones**, because **competitors are already winning with hand-picked curation, quality-seeking subscribers like Tom are leaving for it, and every month we wait the "warehouse" perception gets harder to reverse.**

## 6. Cold-read self-review

_Read your hook back as a skeptical stakeholder. If you don't feel the urgency, that's your data._

| Question | Your answer |
|---|---|
| Is the business risk high-stakes enough to justify a new initiative? | High-stakes: a plateau in a subscription business leads to churn and pricing pressure. Current evidence is one churned subscriber (Tom); baseline engagement and churn metrics are needed in Module 3 to prove scale. |
| Is the moment of misery systemic, or just an edge case? | Systemic: it hits the core action (choosing what to watch) every session, and a bigger catalog makes it worse. Confirmed across the sample research (UXR-01, UXR-03, UXR-04, UXR-10, UXR-12). |
| Does the value proposition actually remove the obstacle? | Yes, if Spotlight replaces the scroll with fewer, explained picks. If it's just another "Top 10" carousel, it's a generic feature. Depends on fixing watchlist sync (BUG-1058) and cross-device resume (BUG-1061) first, or saved picks get lost. |

### Known risks and how the strategy answers them

| Risk a skeptic will raise | Our answer |
|---|---|
| "Why not just fix the bugs?" | Bugs lose viewers *after* they choose; curation loses them *before* they choose (Priya, Aisha and Marcus never press play). Sync and resume fixes (BUG-1058, BUG-1061) become **Phase 0** of Spotlight, not a competing priority. |
| Human curation can't be personalized at scale | **Hybrid model:** editors choose and annotate a pool of 100–200 standout titles a month; the algorithm only matches that pool to each viewer. Trust comes from the editors, personalization from the matching. |
| The catalog may not have enough gems | Before launch, an editor audits the catalog for 50+ Spotlight-worthy titles, including restored older titles. If the audit fails, the problem is content, not discovery. |
| Lapsed viewers never open the app | Two goals: **retain** at-risk subscribers in the app, and **win back** lapsed ones with a weekly Spotlight email (the channel that already won Tom). |
| The discerning segment may be small | The Curator-Seeker is the *design* persona; the same "fewer, explained picks" also serves the larger Overwhelmed Evening Viewer segment (Priya, Aisha, Beth, focus group). |
| "Every streamer has a Top 10 row" | Spotlight replaces the scroll instead of adding a row, explains every pick, and draws on a 15,000-title catalog a two-film newsletter can't match. |
| Viewers won't rate picks | Learn from passive signals (finished, abandoned, saved, skipped); ratings are optional. |

## 7. Finalized hypothesis _(complete in Module 3)_

> Based on [qual + quant evidence], I believe that [solving X] for [persona] will result in [outcome], as measured by a [X%] change in [success metric]. I will protect [guardrail metric] and make a go/no-go decision after [decision window].

## Link to full artifact

Completed directly in this repo; see sections 1–6 above.
