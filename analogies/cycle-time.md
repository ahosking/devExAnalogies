## 🚴 Cycling Analogy: Cadence + Power = Speed

**The Core Concept:**

In cycling, your speed is the product of two independent variables:

`
Speed = Cadence (RPM) × Power (watts per pedal stroke)
`

A cyclist can go fast by:

- Spinning fast with moderate power (high cadence, lower power)
- Pedaling slowly with tremendous force (low cadence, high power)
- Balancing both (optimal cadence + sufficient power)

**The Developer Productivity Parallel:**

`
True Productivity = Cycle Time (how fast) × Impact/Quality (how valuable)
`

| Metric | Cycling Term | Developer Equivalent | What It Measures |
|--------|--------------|----------------------|------------------|
| **Cadence** | RPM (revolutions per minute) | Cycle Time / Throughput | How *frequently* code ships |
| **Power** | Watts per pedal stroke | Impact, Quality, Complexity | How *meaningful* the work is |
| **Speed** | MPH (miles per hour) | True Productivity | Actual value delivered |

**Why This Matters:**

### ❌ The Problem with Cycle Time Alone

If you optimize **only for cadence** (fast cycle time):

- Teams ship trivial changes constantly
- PRs get smaller and smaller to reduce review time
- High throughput, but low impact
- Like spinning your bike wheels fast while stuck in traffic

**Real Example from Transcript:**

> "Cycle time is measuring so many different things and so many different actual different instances in workflows and ways that when an organization just looks at cycle time, I don't think it actually provides a lot of information."

### ✅ The Solution: Balance Both Dimensions

You need to measure **and optimize for both**:

- ✅ Reasonable cycle time (not shipping is also bad)
- ✅ High-impact work (not just high volume)
- ✅ Code quality (not rushed shipping)

**Real Example:**

`
Scenario A: 10 PRs/week, 1 hour cycle time each
→ High cadence, but are they meaningful changes?

Scenario B: 2 PRs/week, 8 hours cycle time each
→ Lower cadence, but more substantial features?

The Answer: It depends on POWER (impact)
→ If B's PRs have 5x the business impact, B wins
`

## 🔧 How to Use This Analogy

### With Technical Teams

> "We want to measure both how fast we ship AND how impactful those changes are. It's like cycling—speed isn't just cadence, it's cadence times power. If we only optimize for fast shipping, we're like a cyclist spinning at high RPM but going nowhere."

### With Executives

> "Think of it like a runner. You can increase your speed by running faster (cadence) or by increasing your stride length (power). But if you only focus on running faster, you might sacrifice stride quality. We need to optimize both."

### When Someone Pushes for "Lower Cycle Time"

> "Cycle time is like cadence—it's part of the picture. But a 1-hour cycle time for a one-line comment is different from a 1-hour cycle time for a major feature. We need to understand what's actually being shipped (power) to know if we're being productive."

## 📊 Metrics Framework Using This Analogy

### Cadence Metrics (How Fast)

- PR throughput (PRs per week)
- Deployment frequency
- Cycle time (from commit to deploy)
- Lead time for changes

### Power Metrics (How Valuable)

- Lines of code changed (hint: not always better)
- Feature complexity / story points
- Business impact (revenue, user engagement)
- Code quality / defect rate
- Testing coverage

### Balance Metrics (Both)

- **Velocity** = Throughput × Quality
- **Impact per cycle** = Changes shipped × Business value
- **Developer experience score** (time to get feedback, unblocked time)

## 🚨 Common Objections & Responses

### "But we can't measure power/impact quantitatively"

**Response:**

> "Correct. That's why we combine quantitative metrics (cadence) with qualitative feedback (power). Developers know if they shipped something meaningful or trivial. We ask them directly."

### "If we optimize for impact, won't cycle time go up?"

**Response:**

> "Maybe temporarily. But the goal isn't to optimize *either one independently*—it's to find the sweet spot where you're shipping meaningful work at a reasonable velocity. Like a cyclist finding their optimal cadence for a sustained hill climb."

### "How do we benchmark this?"

**Response:**

> "Benchmarking only cadence is dangerous because organizations have different 'power' requirements. A fintech company shipping security updates has different power needs than a social app. Instead, we look at *each organization's* cadence+power ratio over time."

## 💡 Key Insights

1. **It's not either/or** — You need both metrics, not choosing one
2. **Context matters** — Different teams may have different optimal balances
3. **Gaming prevention** — Optimizing for both simultaneously is much harder to game
4. **Health ranges exist** — Like cycling, there's an optimal zone (not infinite speed)
5. **Messaging is everything** — Frame as "shipping meaningful work faster" not "ship more code"

## 🎯 When to Use This Analogy

✅ **Good for:**

- Explaining why single metrics fail
- Technical audiences who understand metaphors
- Convincing teams to care about quality alongside speed
- Reframing conversations away from "lower cycle time at all costs"

⚠️ **Use with caution:**

- Very senior non-technical executives (might prefer simpler frames)
- In writing-heavy contexts (better in conversations)
- When you need quick buy-in (takes a minute to explain)

## 📚 Related Concepts

- **Input vs. Output Metrics** — Cadence is output; actual development work is input
- **Goodhart's Law** — Optimizing cadence alone is a Goodhart example
- **Healthy Ranges** — Like blood tests, there's a range, not a target
- **Portfolio Approach** — Measure multiple dimensions (cadence + power + quality)

**Status:** 🔄 In development - refine with more specific developer examples  
**Suggested Next Steps:**

- Add real metrics examples from specific organizations
- Create visual diagrams comparing high-cadence/low-power vs. balanced approaches
- Develop variations of this analogy for different audiences
