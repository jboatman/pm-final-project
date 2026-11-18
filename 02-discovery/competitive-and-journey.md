# Competitive Analysis & Journey Map

> **Module 2 · Lab 2 — ★ Deliverable 2.** Repo file `02-discovery/competitive-and-journey.md` — part of your submission.
> Do the lab in the **Module 2 · Exercise 2 Guide** (linked from the Module 2 deck), then click **⬇ Download .md** — it saves as this exact file. Commit it here.
> It becomes the **Competitive Analysis & Journey Map** slide of your Module 6 final deck. Builds on your `ai-synthesis.md` and your Module 1 `problem-hook.md`.

## Responses

- **Role, who are you solving for?:** The Discerning Curator-Seeker: a film-literate viewer in their 40s–50s who sees watching as a deliberate choice, not background noise, and judges the platform by the quality of its picks.
- **Goal, what is this user ultimately trying to achieve?:** To find a hidden gem that fits their particular taste, recommended by a source they trust, without digging through a sea of sequels.
- **Friction, the main barrier (moment of misery) stopping them:** "Because you watched" served Marcus three more action sequels after he watched one ("I'm not a genre, I'm a person"). Searching for "slow quiet French drama" returned a Fast & Furious film. With no trusted curation, Tom cancelled and now watches both films a competitor emails him each week.
- **External tools the user is forced to use:** A competitor's curated service (e.g., a weekly "two hand-picked films" email) and personal recommendations from friends, which they then look up by exact title in StreamLine search.
- **The process, the 3–5 manual steps they take:**
  1. Opens StreamLine, sees "Because you watched" full of the same franchise, and gives up on the home screen.
  2. Leaves the app to get a recommendation they trust, from a friend or a competitor's curated email.
  3. Comes back and searches the exact title, because descriptive searches like "slow quiet French drama" don't work.
  4. Adds it to My List on their phone, then can't find it on the TV because the watchlist doesn't sync, so the effort is lost.
  5. After repeating this enough times, cancels and switches to the competitor that does the curation for them.
- **Core frustration, where the process feels most "broken":** Right after watching one action film, "Because you watched" offers three more sequels from the same franchise, and a search for "slow quiet French drama" returns a Fast & Furious film. In that moment the user realizes StreamLine doesn't understand their taste and that they'll have to look outside the app to find anything good.
- **The evidence, a quote or behavior from the research:** Marcus (UXR-02, 41, film buff): *"The 'Because you watched' row is a joke, it recommended three more action sequels because I watched one. I'm not a genre, I'm a person. I miss when a human curator would surface a hidden gem."* BUG-1091 (Sev: High) confirms the row recommends near-duplicate titles from the same franchise. Tom (UXR-04, lapsed subscriber) cancelled and now watches both films a competitor emails him each week.
- **Journey map, a shareable link or the map file you committed:** [`02-discovery/journey-map.html`](journey-map.html) · [Shareable link](https://claude.ai/artifact/SLDY1AmoRdC8F9bKyiLXNy)

## Competitive landscape: the curation leaders

_Sources: my competitive research notes (Lifehacker, A Good Movie to Watch, Consumer Reports), summarized._

| Service | How it curates | What it tells us |
|---|---|---|
| **Criterion Channel** | Thematic programming, director spotlights, double features, commentary, 24/7 livestream | Human programming works, but it depends on a prestige catalog we don't have. |
| **MUBI** | Hand-picked independent, world and festival films in a curated rotation, plus editorial writing | A small, rotating set is the opposite of the 15,000-title scroll. Editorial writing is part of the product. |
| **Kanopy** | Large indie, international and classic catalog with curated tags and collections, via libraries | Collections and tags help viewers browse a big catalog, but nothing is personalized. |

### The gap Spotlight fills

| | Same for everyone | Personalized |
|---|---|---|
| **Human / editorial** | Criterion, MUBI, Kanopy | **Spotlight** |
| **Algorithmic** | "Top 10" rows | Big-platform recommendations (our sequel loop) |

The leaders curate for self-selected cinephiles, and every subscriber sees the same programming. No one offers editorial curation that's personalized and built for a mainstream audience. Spotlight's position: **Criterion-style curation for viewers who aren't cinephiles, matched to their taste and labeled with a source they trust.**

### Patterns we borrow
- **Double features → a fix for the sequel loop:** editor-paired follow-ups replace "Because you watched" (UXR-02, BUG-1091).
- **Themes → mood browsing:** weekly themes like "Quiet Sundays" answer Beth's request (UXR-09).
- **Director and guest spotlights → borrowed credibility:** named critics or creators curate a Spotlight week.
- **Small rotations → fewer choices:** answers the focus group's "just tell me what's good tonight" (UXR-12).
- **Editorial writing → the "why this, why now" note.**

### Where we can't compete
The leaders' catalogs are part of their curation. StreamLine's catalog is described as "mid-tier," so Spotlight should not try to out-Criterion Criterion. Editors pick the best of each kind, and a pre-launch audit checks that the catalog has enough standout titles.

### Emerging persona (hypothesis): the Critic-Loyalist
A viewer who skips every in-app recommendation and trusts one named source (for example, a four-star RogerEbert.com review). They won't trust a new "StreamLine Editors" label, but they'd act on their critic's rating if it appeared on the pick. This comes from one viewer's experience, not the sample research; it echoes Sam (UXR-10), who trusts friends over the algorithm. Validate before treating it as a segment.

## Trusted sources: who viewers trust, and how they enter the algorithm

_From a team discussion, based on general industry knowledge. Not yet checked against the research or verified with sources._

### What makes a source trusted
People trust a curator when it has a **name** (someone is accountable), **consistency** (you learn whether its taste matches yours), **reasons** (it says *why*), **selectivity** (a short list shows someone filtered) and **independence** (it isn't just promoting what it's paid to promote). StreamLine's "Because you watched" row has none of these, which is why viewers in the research trust friends (Sam, UXR-10), a competitor's newsletter (Tom, UXR-04) or a human curator (Marcus, UXR-02) over it.

| Source | Why viewers trust it | How it enters Spotlight | Catch |
|---|---|---|---|
| **Named critics** (e.g., RogerEbert.com) | A consistent voice, a simple star scale, reasons in every review | Filter the pool (3½★+), label the pick, Critic-backed lens | Licensing; older and obscure titles often lack reviews |
| **Critic aggregators** (Rotten Tomatoes, Metacritic) | Many critics combined into one quick score | Filter the pool | Licensing; says nothing about personal fit; favors widely reviewed films |
| **Festivals and awards** (Cannes, Sundance, TIFF, Oscars) | Expert juries and prestige | Filter the pool, label ("Sundance selection") | Public facts, so cheap to use, but skews toward art-house films |
| **Studio or label brands** (e.g., A24, Criterion) | The brand is the taste signal | Label, and a "follow" option in setup | Covers only the titles we license from them |
| **Community ratings** (e.g., Letterboxd) | Ratings and lists from viewers who care about film; you can follow people whose taste matches yours | Matching input; inspiration for following other viewers | Data isn't freely available; would need a partnership |
| **StreamLine editors** | Writes the "why this, why now" note; covers back-catalog gems critics skipped | Filter the pool, tag titles, label the pick | Cost; must earn trust from scratch; risk of skewing artsy |
| **Our own viewer signals** | "Viewers with your taste finished this" | Matching input and the "Viewers love this" label | Takes time to build; needs passive signals (finished, saved, skipped), not star ratings |

### Five ways trusted sources feed the algorithm
1. **Filter:** only titles a trusted source endorsed can enter the Spotlight pool (critic rating, festival selection, editor pick, viewer favorite).
2. **Tag:** editors tag titles by feel ("slow-burn," "cozy," "twisty"), and matching uses those tags. Netflix famously paid people to tag its catalog by hand, and those tags powered its micro-genres. This is how human judgment shapes matching without the viewer seeing it.
3. **Label:** the pick shows who vouches for it ("★★★★ RogerEbert.com," "Editors' pick"). This is what turns the algorithm's pick into a trusted one.
4. **Follow:** in setup, the viewer chooses the sources they trust (a critic, a brand, editors), like following people on Letterboxd. This extends the lens.
5. **Learn:** our own signals (finished, saved, skipped) feed back into matching, and over time "viewers like you" becomes a trusted source of its own.

**Precedent:** Spotify pairs human-edited playlists with algorithmic personalization. Editors set the playlists and the algorithm adapts them to each listener, which is the model Spotlight follows.

**Open questions:** which sources are worth licensing, and does a source label actually raise play-through? Test the labels in interviews (Module 3) and run an A/B test with labels on and off (Module 5).
