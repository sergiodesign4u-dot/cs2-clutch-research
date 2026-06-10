# AARRR Model

**v1 - pre-research hypotheses**
Created: 2026-06-10. Targets labeled as hypotheses. To be validated against competitor and benchmark research.

---

## Acquisition

### Channels and Mechanics

**Influencer and streamer seeding (primary):** CS2 streamers on Twitch and YouTube are the highest-trust channel in this market. A streamer opening cases on-stream creates authentic content and direct traffic. Gifting free cases to streamers with no scripted outcome is the trust-preserving approach.

**Affiliate and referral network:** Players refer other players via unique links. Revenue share or flat bonus per referred depositor. The Grinder segment is the natural affiliate, but any user can participate.

**Organic search and content:** Skin value comparison, odds analysis, and "how to get [specific skin]" content targets the Collector segment who researches before spending.

**Social sharing (viral loop):** Big drops and battle wins shared via screenshot or clip. Platform must make sharing trivially easy. Twitter/X and Discord are the primary sharing surfaces for CS2 culture.

**Paid social:** Targeted to CS2 players on YouTube pre-roll and Reddit. Cost-efficient for prospecting but less trusted than peer referral in this category.

### Key Hypotheses

1. Influencer seeding with authentic play (no scripted outcomes) will drive more durable trust than paid promotion, because the CS2 community is highly sensitive to shill content.
2. Affiliate links from Grinder-segment players to their community will have higher conversion rates than cold paid traffic, because referral implies social proof.
3. SEO targeting "CS2 case odds" and "how to get [skin name]" keywords will organically capture Collector-segment users in high-intent research moments.

### What is Unknown

- Cost per acquired depositor across channels (no data until live)
- Which streamer tier (micro vs. macro) produces better LTV users
- Whether paid social in this category is restricted by platform policies (Google, Meta have restrictions on gambling-adjacent ads)

### Primary Metric

First-time depositors per week. Target: [?] (hypothesis, to benchmark against competitor public figures if available).

### MVP Product Decision

Build referral link generation and basic affiliate dashboard in MVP. Do not build a full affiliate program before launch - manual seeding and referral links are sufficient to test the channel.

---

## Activation

### Channels and Mechanics

**No-deposit starter case (hypothesis):** A free or low-cost first case to let users experience the reveal without deposit risk. Lowers the barrier to the primary JTBD. Must be designed so it does not produce withdrawal-eligible value (to prevent abuse) but does produce a real reveal experience.

**First-deposit bonus:** A percentage match on the first deposit converts interest to committed spend. Bonus balance with wagering requirements is the standard mechanic in adjacent markets.

**Onboarding flow:** New user lands on a page that shows live drops, explains provable fairness in one sentence, and gets to a case in under 3 clicks. Friction between landing and first open must be minimal.

**Age-gate and verification:** Required before any case interaction. Must not feel punitive - it is a trust signal as much as a compliance requirement.

### Key Hypotheses

1. A no-deposit first case (producing non-withdrawable outcome) will increase activation rate by 15-25% relative to a deposit-only flow, because it lets the Thrill Seeker experience the product before committing money.
2. First-deposit bonus match of 100% (if achievable within margin) will outperform 50% match in activation rate, all else equal.
3. Users who complete a provable-fairness verification in their first session have higher D7 retention, because trust is established early.

### What is Unknown

- Optimal wagering requirement on the first-deposit bonus (too low = margin loss, too high = user feels trapped)
- Whether age-gate friction (ID verification) meaningfully reduces activation vs. simple birthday entry
- The minimum viable deposit amount that activates Thrill Seekers vs. Grinders (different thresholds expected)

### Primary Metric

First open completion rate (users who arrive and complete at least one case open). Target: [?] 40-60% of registered users (hypothesis).

### MVP Product Decision

Build the full opening experience first - it is the primary activation event. Bonus and referral mechanics can be simplified for launch. Age-gate is non-optional and must ship in MVP.

---

## Retention

### Channels and Mechanics

**Case battles as a return driver:** Battles require opponents, which means waiting for a lobby to fill. This creates a scheduling behavior - users return to see if their battle is starting. Notification triggers (battle starting, battle result) are high-intent re-engagement moments.

**Upgrades as a progression loop:** Users who receive a low-value skin from a case may immediately attempt an upgrade. The upgrade path creates a session extension mechanic. Users who hit a good upgrade have a reason to share, which feeds Acquisition.

**Daily or weekly case bonuses:** A free or discounted case on a cadence (daily login bonus, weekly loyalty case) is a low-cost retention mechanic used across the adjacent category. It brings Grinders back on cadence.

**Rakeback payout notifications:** Informing a Grinder that they have earned rakeback credits and can claim them is a re-engagement trigger with direct monetary value. Hypothesis: this is a highly effective push notification.

**Win sharing and social proof:** Users who share a win bring back themselves (pride, validation) and potentially bring new users. The platform must make sharing a first-class feature, not an afterthought.

### Key Hypotheses

1. Case battles will be the primary retention driver for Thrill Seekers because they add competitive stakes and social interaction to the core opening loop.
2. Upgrade paths directly after a case open (in the same session) will extend session length by 30%+ for Collectors and Grinders who receive a sub-target outcome.
3. A daily login bonus (free low-value case or extra credits) will improve D7 retention by 10-15 percentage points, based on analogy with adjacent products - hypothesis to validate.

### What is Unknown

- Optimal battle lobby size (2-player vs. 4-player vs. larger) for fill speed vs. excitement
- Whether push notifications are permitted in the target markets and whether users opt in at meaningful rates
- How fast the upgrade catalogue must iterate to prevent Grinders from feeling they have "solved" the optimal path

### Primary Metric

D7 retention rate. Target: [?] 35%+ (hypothesis). Secondary: sessions per active user per week. Target: [?] 3+ (hypothesis).

### MVP Product Decision

Ship battles with 2-player lobbies first (fastest to fill, simplest to build). Add 4-player and multi-case battle formats based on retention data. Daily bonus is a low-effort high-impact feature - include in MVP.

---

## Revenue

### Channels and Mechanics

**House edge on cases (primary):** Every case opened has an expected value below 100% of its cost. The gap is the gross gaming revenue (GGR). Volume times edge equals revenue. The platform controls edge through case design - specifically, the probability distribution of outcomes relative to their skin market values.

**House edge on battles:** Battles run on the same case math. All participants open cases from the same pool; the winner takes all outcomes. The edge is already baked into the cases opened, not a separate fee. Some platforms add a 1-3% pot fee on top of the case edge - hypothesis to validate against competitor research.

**Deposit bonus wagering requirement as margin protection:** Bonus balance that requires X times wagering before withdrawal is not revenue itself, but it extends play long enough for the edge to apply multiple times. If a user deposits $100, receives $100 bonus, and must wager 5x before withdrawal, the edge applies to $1000 of action - at a 30% edge, that generates $300 GGR before any withdrawal is possible from the bonus portion.

**Referral bonus cost vs. LTV:** Referral commissions (5-15% of referred user's GGR) are a cost, but referred users are cheaper to acquire than paid traffic. Positive if LTV exceeds acquisition cost plus referral cost.

**Rakeback as a margin-sharing mechanic:** Returning a percentage of GGR margin to high-volume users reduces net margin per user but extends LTV. A Grinder who receives rakeback and continues playing generates more total GGR than a Grinder who churns due to feeling the edge is too high.

### Key Hypotheses

1. A house edge of 25-40% on cases (meaning case expected value is 60-75% of face price) is within market range and sustainable - hypothesis to validate against published competitor odds.
2. The rakeback mechanic, if set at 10% of the platform's GGR margin, will increase Grinder LTV by more than the cost of the rebate, because it reduces churn in the highest-volume segment.
3. The tension between bonus generosity (high activation) and margin erosion (lower GGR per user) will require calibration over the first 90 days. Starting with conservative wagering requirements is safer than starting too loose.

### Tension: Generosity vs. Margin

This is the central economic tension of the product. Better user conditions (higher bonus match, lower wagering requirements, rakeback) improve activation and retention but reduce net margin per user. The hypothesis is that the LTV increase from better retention outweighs the margin reduction - but this requires live data to validate. Phase 3 competitor research will inform where the current market sets these levers.

### What is Unknown

- Market-standard case edge percentage (range and norms)
- Whether a battle pot fee is standard or seen as negative by users
- Minimum viable margin after bonuses and rakeback that sustains the business

### Primary Metric

Gross gaming revenue (GGR) per depositing user per month. Target: [?] (hypothesis, requires market data).

### MVP Product Decision

Launch with clearly designed case mathematics (defined edge) before building bonus and rakeback systems. Understand the baseline GGR per user before layering incentives on top. Rakeback is a Phase 2 feature after launch, not MVP.

---

## Referral

### Channels and Mechanics

**Steam and Discord as natural surfaces:** The CS2 community lives on Discord servers, Steam groups, and CS2-adjacent subreddits. These are the surfaces where skin content is shared organically. The platform should be built to generate content that travels on these surfaces.

**Streamer affiliate program:** Streamers with dedicated CS2 or skin-focused audiences are the most efficient referral channel. They create content and send it to their audience. A tiered affiliate commission (revenue share for larger streamers, flat bonus for smaller) is the hypothesis.

**User referral links:** Every registered user gets a referral link. Referred users trigger a bonus for both parties - the referrer gets a balance credit or commission, the referred user gets a first-deposit bonus on top of the standard offer.

**Win sharing as organic referral:** A big drop or battle win shared on Twitter/X or Discord functions as organic referral. The share creates a link back to the platform. The more dramatic and clip-worthy the reveal, the more likely it travels. This makes the reveal animation quality directly tied to acquisition.

**CS2 community events:** Sponsoring tournaments, funding community events, or running platform-hosted tournaments (battle ladder, etc.) embeds the brand in the community rather than advertising to it.

### Key Hypotheses

1. Win sharing from the Thrill Seeker segment will be the primary source of organic referral, because this segment has the highest tendency to share screenshots and clips of big drops.
2. The referral loop will be stronger on Discord than on other platforms, because CS2 skin culture is concentrated there.
3. A two-sided referral bonus (referrer AND referred both receive value) will outperform a one-sided bonus, because the referred user has an additional reason to deposit.

### What is Unknown

- Which streamers are available and at what cost per deal
- Whether Google, YouTube, or Twitch restrict promotional content from this category
- Optimal referral commission rate that motivates affiliates without eroding margin

### Primary Metric

Referred depositors as a percentage of total new depositors. Target: [?] 20-35% of new depositors from referral (hypothesis).

### MVP Product Decision

Build basic referral links and tracking from day one. A full affiliate dashboard can come later. The most important thing is that sharing a win generates a referral link, not that the dashboard is polished.

---

## Summary Metrics Table

| Stage | Primary Metric | Target (hypothesis) | Why it matters |
|-------|---------------|---------------------|----------------|
| Acquisition | New registered users per week | [?] | Baseline for all funnel stages |
| Acquisition | Cost per first depositor | [?] | Governs channel mix and budget allocation |
| Activation | First open completion rate | [?] 40-60% of registered | Primary activation event quality |
| Activation | Visitor-to-first-deposit rate | [?] 8-15% | Conversion health |
| Retention | D7 retention rate | [?] 35%+ | Early engagement and loop quality |
| Retention | Sessions per active user per week | [?] 3+ | Depth of engagement |
| Revenue | GGR per depositing user per month | [?] | Core economic health |
| Revenue | Bonus burn rate vs. GGR | [?] | Margin health |
| Referral | Referred depositors / total depositors | [?] 20-35% | Community channel efficiency |

All targets are hypotheses. Replace with real benchmarks when competitive research data is available.

---

## Key Takeaways

1. The case opening reveal is the single most important product moment. Activation, retention, referral, and revenue all flow from the quality of this one experience. It must be fast, dramatic, and unambiguously fair.

2. Case battles and upgrades are retention mechanics, not acquisition mechanics. They extend sessions and bring users back. Build them for the Grinder and the Thrill Seeker who has already opened. They should not be the first thing a new user sees.

3. The economic model has a built-in tension between user generosity (which improves LTV) and margin (which sustains the business). The right balance requires live data. Launch with conservative bonuses and tighten or loosen based on early cohort behavior, not hypotheses.

4. Trust is not just a design principle - it is the acquisition and referral engine. A user who believes the drop is fair shares the win. A user who suspects it is rigged churns and warns others. Every product decision should be evaluated against the question: does this make the platform feel more or less trustworthy?
