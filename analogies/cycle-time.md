## Cycling Analogy: Cadence + Power = Speed

In cycling, speed comes from two independent variables:

```text
Speed = Cadence (RPM) x Power (watts per pedal stroke)
```

A cyclist can go fast by spinning fast with moderate power, pedaling slowly with tremendous force, or finding the balance between the two. None of these is inherently right. It depends on context.

**The developer productivity parallel:**

```text
True Productivity = Cycle Time (how fast) x Impact/Quality (how valuable)
```

| Metric | Cycling Term | Developer Equivalent | What It Measures |
| ------ | ------------ | -------------------- | ---------------- |
| Cadence | RPM | Cycle Time / Throughput | How frequently code ships |
| Power | Watts per pedal stroke | Impact, Quality, Complexity | How meaningful the work is |
| Speed | MPH | True Productivity | Actual value delivered |

### The problem with cycle time alone

If you optimize only for cadence, teams start shipping trivial changes constantly. PRs get smaller and smaller to reduce review time. Throughput goes up while impact goes down. It's like spinning your bike wheels fast while stuck in traffic.

> "Cycle time is measuring so many different things and so many different actual different instances in workflows and ways that when an organization just looks at cycle time, I don't think it actually provides a lot of information."

### What to actually optimize for

You need both:

- Reasonable cycle time (not shipping is also bad)
- High-impact work, not just high volume
- Code quality, not rushed shipping

```text
Scenario A: 10 PRs/week, 1 hour cycle time each
-> High cadence. But are they meaningful changes?

Scenario B: 2 PRs/week, 8 hours cycle time each
-> Lower cadence. But more substantial features?

It depends on impact. If B's PRs have 5x the business impact, B wins.
```

## Using this analogy

**With technical teams:**
> "We want to measure both how fast we ship and how impactful those changes are. It's like cycling: speed isn't just cadence, it's cadence times power. If we only optimize for fast shipping, we're like a cyclist spinning at high RPM but going nowhere."

**With executives:**
> "Think of it like a runner. You can increase speed by running faster (cadence) or by increasing stride length (power). Focusing only on running faster might sacrifice stride quality. We need to optimize both."

**When someone pushes for lower cycle time:**
> "Cycle time is like cadence: part of the picture. But a 1-hour cycle time for a one-line comment is different from a 1-hour cycle time for a major feature. We need to understand what's actually being shipped to know if we're being productive."

## Metrics

**Cadence (how fast):**

- PR throughput
- Deployment frequency
- Cycle time (commit to deploy)
- Lead time for changes

**Power (how valuable):**

- Feature complexity
- Business impact (revenue, user engagement)
- Code quality and defect rate
- Testing coverage

**Balance (both):**

- Velocity = throughput x quality
- Impact per cycle = changes shipped x business value
- Developer experience score (time to get feedback, unblocked time)

## Common objections

### "We can't measure power or impact quantitatively"

> "Correct. That's why we combine quantitative metrics (cadence) with qualitative feedback (power). Developers know if they shipped something meaningful or trivial. We ask them directly."

### "If we optimize for impact, won't cycle time go up?"

> "Maybe temporarily. The goal isn't to optimize either one independently. It's to find the sweet spot where you're shipping meaningful work at a reasonable velocity. Like a cyclist finding their optimal cadence for a sustained hill climb."

### "How do we benchmark this?"

> "Benchmarking only cadence is dangerous because organizations have different power requirements. A fintech company shipping security updates has different needs than a social app. Look at each organization's cadence+power ratio over time, not against an industry number."

## Key points

1. It's not either/or. You need both metrics.
2. Context matters. Different teams may have different optimal balances.
3. Optimizing for both simultaneously is much harder to game.
4. Like cycling, there's a healthy zone, not a number to minimize forever.
5. Frame it as "shipping meaningful work faster," not "ship more code."

## When to use this

Works well:

- Explaining why single metrics fail
- Talking with technical audiences who respond to metaphors
- Convincing teams to care about quality alongside speed
- Reframing away from "lower cycle time at all costs"

Use with caution:

- Very senior non-technical executives (might prefer simpler frames)
- When you need quick buy-in (takes a few minutes to explain well)

## Related

- [Input vs. Output Metrics](input-output-metrics.md): cadence is an output metric; actual development work is input
- Goodhart's Law: optimizing cadence alone is a textbook example
- [Health Analogies](health.md): like blood tests, metrics have healthy ranges, not infinite targets
