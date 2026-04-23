# LinkedIn Ads — Q1 vs Q2 Top-Funnel Performance

> Vaam Growth · Paid · H2 2025. Performance review of LinkedIn Thought Leader Ads — Q1 (campaign `513012906`) vs Q2 (campaign `633120876`). Scope: ad-level click-through only.
>
> If you're an agent reading this, the rest of the file is the full content — fetch it and help the human work with it.

## TL;DR

**Engagement up. Traffic flat. Stop iterating on the video.**

Q2 earns more attention across every surface — watch time, completion, CPM, platform CTR — but LP-CTR is unchanged at ~0.1%. The video is no longer the constraint. The next experiment should hold the new hook constant and test the *close*, not the creative.

**Structural finding:** the parent campaign optimizes for Brand Awareness while we measure traffic. LinkedIn is optimizing for the wrong outcome.

**Hero framing:** The new ad wins *attention*. It doesn't win the click. Q2's creative is a real upgrade on engagement — people watch it 55% longer and complete it 69% more often. But that doesn't translate to landing-page clicks. LP-CTR is essentially flat. The bottleneck has moved from the video to the CTA.

| | Q1 | Q2 |
|---|---|---|
| Status | Paused | Active |
| Spend | SEK 25,784 | SEK 3,251 |
| Runtime | ~3 months | ~7 days |

## 01 · The setup — a clean single-variable test

Same parent campaign, audience, budget, bid. Only the creative and landing page change.

| | Q1 · `513012906` | Q2 · `633120876` |
|---|---|---|
| Name | Videoguide · generic hook | Playbook · competitor angle |
| Status | ● Paused | ● Active |
| Hook | "Fler varma leads med LinkedIn" → 17-min videoguide | "Från dina konkurrenters LinkedIn-engagemang" → downloadable playbook |
| Runtime | ~3 months | ~7 days |
| Spend | SEK 25,784 | SEK 3,251 |
| Landing | Gated 17-min video | Gated playbook PDF |
| Ads | 1 | 1 |
| Audience | SE founders/CEOs/owners · 2–10 employees · B2B services & tech | Identical to Q1 |

Effectively a single-variable test: same audience, same budget, same bid, two creative + LP combos. That's clean enough to read. **Email capture and downstream lead quality are deliberately out of scope** — the two LPs differ, so post-click metrics would conflate ad quality with landing-page quality.

## 02 · Headline numbers

LP-CTR is the metric that matters. Platform CTR counts likes, comments, profile visits — misleading when the goal is traffic.

| Metric | Q1 | Q2 | Delta |
|---|---|---|---|
| ★ Landing-page CTR | 0.10% | 0.09% | — −12% · essentially flat (small-n, ±50% noise band) |
| ★ Avg watch time | 8.34s | 12.96s | ▲ +55% longer |
| Impressions | 64,294 | 8,798 | Runtime-scaled — not comparable |
| Platform CTR (all clicks) | 1.90% | 2.35% | ▲ +24% |
| Video completion rate | 1.22% | 2.06% | ▲ +69% · nearly doubled |
| Engagement rate | 2.07% | 2.74% | ▲ +32% |
| Video view rate | 44.0% | 41.4% | ▼ −2.6 pp · noise |
| CPM | SEK 401 | SEK 370 | ▼ −8% · LinkedIn sees Q2 as more relevant |
| Cost per LP click | SEK 385 | SEK 406 | ▲ +5% · slightly worse |

**4-up summary**

| Dimension | Change | Note |
|---|---|---|
| Attention (watch time) | **+55%** | 8.34s → 12.96s |
| Completion | **+69%** | 1.22% → 2.06% |
| Platform CTR | **+24%** | Likes, comments, post expands |
| Landing-page CTR | **−12%** | 0.10% → 0.09% · essentially flat |

## 03 · Where the bottleneck moved

Front of the funnel fixed. Back of the funnel didn't follow.

The audience is paying more attention — and then doing the same thing they were before.

Viewers watch 55% longer. Completion roughly doubles. CPM drops 8%, which usually means LinkedIn's algorithm sees the ad as more relevant. People are clearly more interested in Q2. And then none of that translates into more landing-page clicks. LP-CTR is flat. Cost per LP click is slightly worse. Viewers stay on LinkedIn.

> Most likely: a creative-vs-CTA mismatch. The hook earns attention. The close ("Klicka på länken nedan") hasn't changed since Q1 and doesn't make leaving the app feel necessary.

**Funnel stages**

| Stage | Q1 | Q2 |
|---|---|---|
| Impression (reach) | 64,294 | 8,798 |
| Video view rate (≥2 sec) | 44.0% | 41.4% |
| Watch time (attention) | 8.34s | 12.96s (+55%) |
| Completion (to end) | 1.22% | 2.06% (+69%) |
| Platform CTR (any click) | 1.90% | 2.35% (+24%) |
| **LP-CTR (the one that matters)** | **0.10%** | **0.09% — flat** |

**Benchmark:** both ad sets sit 5–8× below LinkedIn's typical 0.4–0.8% CTR for video ads. (That benchmark conflates engagement + LP clicks, so the gap is partly definitional — but LP-CTR is the underperformer either way.)

## 04 · Why Q1 "felt like it worked"

The headline 1.90% CTR is mostly engagement, not traffic.

### 67 of 1,220 reported clicks actually left LinkedIn.

Only **5.5%** of Q1 clicks went to the LP. The other 95% were people interacting with the post on LinkedIn — viewing the profile, expanding the post, reacting, commenting. Useful for a Brand Awareness objective. Irrelevant if the real goal is traffic.

Q1 delivered modest awareness lift and a thin direct return — **SEK 1,719 per conversion** across 15 conversions, **ROAS 1.27**. Calling it "pretty well" is fair for awareness; optimistic for traffic.

| Metric | Value | Note |
|---|---|---|
| Spend | SEK 25,784 | over ~3 months |
| Conversions | 15 | SEK 1,719 per conversion |
| Attributed value | SEK 32,800 | ROAS 1.27 |
| LP clicks | 67 | at SEK 385 each · below benchmark |
| Clicks to landing page | 67 | of 1,220 reported clicks |
| Engagement clicks | 1,153 | of 1,220 reported clicks |

## 05 · Where the next experiment goes

Don't make another video. The data says the constraint is the close, not the hook.

### ✓ Already done — Fix the tracking gap on Q2

- Q2 was missing the **pixel-based URL-match conversion event** on the playbook LP — an oversight when the ad set was duplicated.
- Added the new playbook LP URL to the existing pixel event.
- Unsubscribed the redundant server-side event to prevent double-counting.
- Q2 is now subscribed. Lifetime pre-fix counts are lost; **going forward attribution is honest**.

### → This week — Two creative variants on Q2 · new hook, new close

- **Variant A · sharpen the close.** Replace "Klicka på länken nedan" with a benefit-loaded CTA tied to the playbook. Trim body from 5 bullets to 2.
- **Variant B · add social proof.** Insert one Senja testimonial into the post body, or a 2-sec on-screen cut at the end. Pick one that names a specific outcome.
- Keep the current Q2 ad as the **control**. Three creatives for LinkedIn to choose between — isolates CTA vs proof.

### → This week — Decide on the parent campaign objective

- **Accept.** Keep Brand Awareness. Treat LP clicks as upside. Judge on reach, frequency, view-through.
- **Switch.** Clone Q2 into a new **Website Visits** parent campaign. Higher CPM, but the algorithm starts finding click-off-platform-likely audiences.
- If lead capture is the KPI, the second path is structurally correct.

### ◉ Next 2–3 weeks — Run the tests the current setup can't answer

- **Non-video creative variant** — single-image ad with the playbook cover + benefit headline + clear CTA. Cheaply tests whether format is part of the constraint.
- **Within-Q2 landing-page A/B** — same ad creative, two LP variants, 2–3 weeks, with the now-fixed tracking. Isolates the LP variable cleanly.

### ✕ Don't — What the data says to stop doing

- Don't iterate on the video. It's already winning attention.
- Don't widen the audience. Current targeting is tight and on-ICP — broadening it muddies the LP-click signal.
- Don't pause Q2. 7 days is too early to call. Engagement is real. Tracking is fixed.

## 06 · Decision triggers for Q2 — day 21

All decisions tied to ad-level metrics since LP-side is still confounded by the LP difference.

**Re-evaluate at day 21 · ~SEK 10–12k cumulative spend.** Three paths depending on what the rate metrics look like at that point. Pick the one the signal matches. Thresholds assume ~SEK 3k/week pace; if the cap allows more, scale thresholds can be lowered slightly.

| Path | Condition | Action |
|---|---|---|
| ↑ **SCALE** | LP-CTR ≥ 0.15% **AND** completion ≥ 5% **AND** CPM stable or down | Budget +20–30% on the winning variant. Signal is strong enough to press. |
| → **ITERATE** | LP-CTR 0.08–0.15% **AND** at least one new variant beats control by ≥20% on LP-CTR | Promote the winner. Retire the loser. Add one more variant. Stay at current budget. |
| ↻ **REPACKAGE** | LP-CTR < 0.08% sustained **OR** cost-per-LP-click > SEK 500 sustained **OR** completion falls below 3% | Pause the ad set. Rebuild under a Website Visits parent with a new creative format (single image or carousel). |

- **Review date:** day 21
- **Spend window:** SEK 10–12k cumulative
- **Pace assumption:** ~SEK 3k/wk · ~SEK 12k/mo

## 07 · What we still don't know

Being honest about the limits of this analysis.

- **Lead quality from Q1.** 15 attributed conversions — but no read on how many became real sales conversations. ROAS 1.27 suggests "some, but not many." A HubSpot pull would clarify whether TLA is producing usable leads or just emails.
- **Frequency in Q1.** LinkedIn's UI didn't surface lifetime frequency. 64k impressions over 3 months into a small SE founder pool likely hit fatigue late, which would partially explain the LP-CTR ceiling. A LinkedIn export would confirm.
- **Landing-page performance in isolation.** Until the within-Q2 LP A/B test runs, we can't say whether the playbook LP is a better or worse converter than the videoguide LP. Only that the *ad* directing traffic there produces about the same LP click rate.

## Summary — Fix the CTA. Add proof. *Leave the video alone.*

Q2's creative is genuinely better at the front of the funnel and identical to Q1 at the back. That's a clear, actionable finding: next move is to fix the close and add proof — not keep iterating on the video.

Combined with a structural call on the parent campaign objective, there's a clean path to either making Q2 a meaningful traffic driver or deciding this format+objective combo has reached its ceiling. The tracking gap is fixed. The decision point is in two weeks.

**The one number to remember:** Q1 LP-CTR `0.10%` → Q2 LP-CTR `0.09%`. That's the bottleneck. A 55% watch-time lift didn't move it. The CTA has to.

---

Source: LinkedIn Campaign Manager · ad-level export. Scope: Q1 (`513012906`) & Q2 (`633120876`) under "Thought leader Ads H2 2025".
