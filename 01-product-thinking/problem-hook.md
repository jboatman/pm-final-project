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

> For **overwhelmed evening viewers who just want something good tonight** (the "Wanderers," 41% of subscribers) and the discerning viewers who share the same pain, we will **replace the 15,000-title scroll with Spotlight: three standout picks a night, each labeled with the trusted source that vouches for it (viewers like them, our editors, or a top critic) and explained ("why this, why now"). A one-tap setup chooses each viewer's lens, with "Easy tonight" as the default and critic-backed picks for film buffs. Delivered in the app for subscribers and by weekly email for lapsed ones**, because **Wanderers churn the most and respond the most to curation (22 pts lower churn when exposed to Spotlight), competitors are already winning with hand-picked picks, and every month we wait the "warehouse" perception gets harder to reverse.**

## 6. Cold-read self-review

_Read your hook back as a skeptical stakeholder. If you don't feel the urgency, that's your data._

| Question | Your answer |
|---|---|
| Is the business risk high-stakes enough to justify a new initiative? | High-stakes: a plateau in a subscription business leads to churn and pricing pressure. Module 3 data confirms scale: mobile DAU is down 21% in six months and sessions reaching 30+ minutes fell from 19% to 11%. |
| Is the moment of misery systemic, or just an edge case? | Systemic: it hits the core action (choosing what to watch) every session, and a bigger catalog makes it worse. Confirmed across the sample research (UXR-01, UXR-03, UXR-04, UXR-10, UXR-12). |
| Does the value proposition actually remove the obstacle? | Yes, if Spotlight replaces the scroll with fewer, explained picks. If it's just another "Top 10" carousel, it's a generic feature. Depends on fixing watchlist sync (BUG-1058) and cross-device resume (BUG-1061) first, or saved picks get lost. |

### Known risks and how the strategy answers them

| Risk a skeptic will raise | Our answer |
|---|---|
| "Why not just fix the bugs?" | Bugs lose viewers *after* they choose; curation loses them *before* they choose (Priya, Aisha and Marcus never press play). Sync and resume fixes (BUG-1058, BUG-1061) become **Phase 0** of Spotlight, not a competing priority. |
| Human curation can't be personalized at scale | **Hybrid model:** licensed critic ratings, editors and viewer favorites build a pool of 100–200 standout titles a month; the algorithm only matches that pool to each viewer's lens and taste, using tags editors add by feel ("slow-burn," "cozy"). Trust comes from named sources, personalization from the matching. See *Trusted sources* in `02-discovery/competitive-and-journey.md`. |
| "Critics have already reviewed everything. Why hire editors?" | Critics are one of the sources, shown as a labeled lens. Editors cover what critics don't: back-catalog gems that were never widely reviewed, and the "why this, why now" note that ties a title to this viewer and this catalog. The leaders in curation (Criterion, MUBI, Kanopy) all use human programming. |
| Curators skew artsy, and not everyone wants art films | Editors pick **the best of each kind**, not the most artistic: a great heist film or rom-com counts. "Easy tonight" is the default lens for everyone. |
| Some viewers only trust one specific critic | The **Critic-backed lens** shows that critic's rating and a pull quote right on the pick, and can filter to 3½ stars or higher. StreamLine becomes the fastest way to act on a source they already trust. *(Hypothesis: comes from one viewer's experience, not the sample research.)* |
| Several lenses could recreate choice overload | The lens is chosen once in a one- or two-tap setup ("How do you usually pick a film?" plus three favorites, with an option to follow a source they trust, such as a critic, a brand or our editors), then adjusted from viewing behavior. Existing subscribers get a one-time "Set up your Spotlight" card. |
| Critic ratings cost money and may not cover our catalog | Licensing is a real cost and dependency. Before committing, count how many of our 15,000 titles have strong critic reviews; if coverage is thin, the Critic-backed lens leans on editors and on festival selections and awards, which are public and free to use. |
| The catalog may not have enough gems | Before launch, an editor audits the catalog for 50+ Spotlight-worthy titles, including restored older titles. If the audit fails, the problem is content, not discovery. |
| Lapsed viewers never open the app | Two goals: **retain** at-risk subscribers in the app, and **win back** lapsed ones with a weekly Spotlight email (the channel that already won Tom). |
| The discerning segment may be small | **Confirmed in Module 3.** Curator-Seekers behave like Power Users (22% of the base, already watch curated content, low churn). The primary persona is now the **Overwhelmed Evening Viewer**, the "Wanderers" segment (41% of the base, 61% trending content, 22 pts lower churn with Spotlight). The Curator-Seeker stays as design inspiration and the Hidden gems lens. |
| "Every streamer has a Top 10 row" | Spotlight replaces the scroll instead of adding a row, explains every pick, and draws on a 15,000-title catalog a two-film newsletter can't match. |
| Viewers won't rate picks | Learn from passive signals (finished, abandoned, saved, skipped); ratings are optional. |

## 7. Finalized hypothesis _(complete in Module 3)_

> Based on [qual + quant evidence], I believe that [solving X] for [persona] will result in [outcome], as measured by a [X%] change in [success metric]. I will protect [guardrail metric] and make a go/no-go decision after [decision window].

## Link to full artifact

Completed directly in this repo; see sections 1–6 above.
