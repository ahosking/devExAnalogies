## Brains in Jars: Developers Are Not Disembodied Cognition

Coined by [Dr. Cat Hicks](https://www.drcathicks.com/) (psychological scientist, author of *The Psychology of Software Teams*), the "brains in jars" model names a stereotype most engineering orgs run on without admitting it: picture the sci-fi scene, a detached pink brain floating in jelly. That is how a lot of developers suspect their org actually thinks about them. Pure cognition, no body, no history, no feelings, no context. Just output.

It is the perfect antagonist for this whole repository, because every bad metric conversation ("more PRs!", "why can't we measure lines of code?") is downstream of the same mistake: treating people as interchangeable problem-solving units and measuring them as if they work in isolation.

### The core claim

In the brains-in-jars model:
- Technical people are isolated individuals. We only care about their cognition.
- Feelings, belonging, and psychological safety are "soft stuff," a nice-to-have at best, actively opposed to real technical work at worst.
- Any developer can drop into any problem and instantly produce perfect code, so learning on the job is a risk to be punished rather than the normal condition of the work.

The reality it ignores: software problem-solving is a *cumulative culture*. Solutions get transmitted socially through pairing, review, mentorship, and shared context. Individual productivity is scaffolded by the group, not extracted from a lone skull in a jar.

### How it maps to the DevEx problem

| Brains-in-Jars Belief | What It Produces | The Reality It Misses |
| --------------------- | ---------------- | --------------------- |
| Developers are interchangeable units | Staffing math that ignores context loss | Knowledge is social and situated; swapping people destroys it |
| Output is all that matters | Ticket-and-story-point theater | People stop experimenting, asking, and sharing what they don't know |
| Social work is an indulgence | Pairing and mentorship deprioritized | Social learning IS the mechanism of solutioning, not a distraction from it |
| The best work comes from a gifted few | Protect the "10x" people, ignore everyone else | At scale, the reliable 10x outlier does not show up in the data |

### The three thinking traps

Dr Hicks names these three signals that an org has a "brains in jars vibe" in her posit::conf 2025 keynote.[^posit] Her Craft Conference talk is written up in the same terms.[^shiftmag]

1. **Brittle productivity.** The belief that the only way to get outcomes is the grind: cramming, all-nighters, heroics. Nobody can actually sustain that, so people *posture*. It becomes the performance of productivity. Dangerous because it looks good for a surprisingly long time before it breaks.[^posit]
2. **The chilly climate trap.** The culture where you are supposed to hold back emotion, stay cold, and equate "less emoting" with "more technical." Hard to name because it is ambient, but corrosive.[^posit]
3. **The lone genius trap.** Excellence as the exclusive province of a gifted few, e.g. the 10x developer. If a handful of outliers drive all the real output, then they are the only ones worth protecting, and anything they do is fine. This is the trap Hicks most enjoys dismantling.[^posit]


### The evidence (cite as hers)

- Across 5,000+ developers and managers in 12+ industries: people in "lone genius" cultures were roughly **twice as likely** to experience AI skill threat. Cumulative cultures (learning + belonging) significantly reduced it.[^posit][^thriving]
- Given large-scale **cycle time** data and an adversarial search for the 10x outlier, the reliable, consistent individual super-producer **did not appear**. What looked like 10x was meaningful variation across tasks, not a stable property of people.[^posit][^mtp]

### The alternative: seed and soil

The opposite of a brains-in-jars culture is a *cumulative* one, where each hard problem is "a riddle we solve together" instead of a duel. Hicks frames the fix with a seed-and-soil metaphor (from social science): developers are seeds with enormous potential, but growth is stunted in toxic soil no matter how talented the seed. Even modest developers flourish in rich soil.[^shiftmag] The underlying theory is set out in her cumulative-culture-of-problem-solving preprint with Ana Hevesi.[^cumulative]

The three nutrients in the soil (the "psychological affordances"):[^shiftmag][^thriving]

- **Learning culture:** questions are praised, failure is dissected constructively, experimentation gets real time.
- **Social acceptance / belonging:** every person is valued as a whole human, not a code machine; failures don't get you ostracized.
- **Self-efficacy:** people believe they can learn and contribute on hard problems, built through autonomy, right-sized challenge, and progress-focused feedback.

## Using this analogy

**With technical teams:**
> "The brains-in-jars model says you're just cognition in a jar, and all that matters is what comes out. But none of us actually work that way. We solve things by talking, pairing, and reviewing. If we starve that, we're optimizing the jar and wondering why the brain stopped learning."

**With executives:**
> "When we treat developers as interchangeable units and measure only output, we get brittle productivity: it looks great on the dashboard right up until the people posturing to hit it burn out. The teams that actually sustain velocity are the ones where learning and belonging are part of the system, not a perk."

**When someone reaches for the 10x developer:**
> "That's the lone-genius trap. When Hicks went looking for the reliable 10x outlier across thousands of developers and thousands of tasks in real cycle-time data, it wasn't there. What's there is variation across problems, not a stable superhuman. If we build the whole org around protecting a myth, we neglect the culture that actually produces good work."[^posit][^mtp]

**When someone calls psychological safety a buzzword:**
> "In a brains-in-jars culture, safety sounds like fluff opposed to 'real' technical work. But the research runs the other way: when people feel belonging and a learning culture, they write better code, take more ownership, and stop hiding what they don't know. Safety is a performance input, not a spa day."[^shiftmag][^anxiety]

## Common objections

### "This is just soft-skills stuff, not engineering."
> "That's the chilly-climate trap talking. The claim is empirical, not sentimental: social learning is the mechanism by which solutions actually spread through a team. Cutting it doesn't make you more technical, it makes your org's knowledge brittle."

### "But some people really are dramatically more productive."
> "People vary, absolutely. The specific claim under fire is the *stable, reliable 10x individual* who out-produces everyone across contexts. That didn't survive contact with large-scale cycle-time data. Most of what we label a 10x person is a 10x *situation*: right context, right support, right problem."

### "We can't afford to slow down for learning culture right now."
> "That's brittle productivity. The grind looks efficient and holds up for a while, which is exactly why it's a trap. You're borrowing against your people the same way you borrow against a codebase, and the interest comes due as burnout, self-censorship, and attrition."

## When to use this

Works well:
- AI-adoption conversations, where identity threat and skill threat are live (this is the sharpest current use)
- Pushback on 10x-developer and "rockstar hire" thinking
- Explaining why per-developer output metrics quietly damage the thing they measure
- Justifying investment in pairing, mentorship, and psychological safety with evidence

Use with caution:
- Don't oversell the numbers as your own; they're Hicks's, cite her
- With very quantitative skeptics, lead with the cycle-time 10x finding before the "belonging" language, or you'll lose them at "feelings"

## Related

- [Input vs. Output Metrics](input-output-metrics.md): brains-in-jars is the belief system that makes output-as-input measurement feel natural
- [Health Analogies](health.md): the athletic-coaching and peak-fitness entries (individual + system performance, cognitive limits) are the same argument from a different door
- [Cycling Analogy](cycle-time.md): the 10x-developer myth is what happens when you treat cadence as a personal trait
- Goodhart's Law: measure a brain-in-a-jar on output and it will posture to hit the number
- Dr. Cat Hicks, *The Psychology of Software Teams* (Routledge, 2026); "Fight for the Human" newsletter; Developer Thriving / AI Skill Threat research; the cumulative-culture-of-problem-solving preprint (Hicks & Hevesi)

## Sources

[^posit]: Cat Hicks, "The Psychology of Technologists," keynote, posit::conf(2025). Transcript/video: <https://opensource.posit.co/resources/videos/2025-11-07_the-psychology-of-technologists-cat-hicks-catharsis-consulting-positconf2025/> — origin of the "brains in jars" model, the three thinking traps (brittle productivity, chilly climate, lone genius), the 5,000+ developer / 12+ industry AI-skill-threat finding, and the cycle-time search that found no reliable 10x outlier.
[^shiftmag]: "Dr. Cat Hicks on Why Developers Feel Anxious At Work," ShiftMag (writeup of her Craft Conference talk): <https://shiftmag.dev/dr-cat-hicks-software-teams-psychology-5357/> — the brains-in-jars fallacy, contest culture, the seed-and-soil metaphor, and the three psychological affordances (learning culture, belonging, self-efficacy).
[^mtp]: "What your developers aren't telling you — Cat Hicks (Psychologist)," Mind the Product: <https://www.mindtheproduct.com/inside-the-minds-of-your-engineers-cat-hicks-psychologist/> — the "brains and jars" model, cycle-time data on individual performance, and metacognitive scaffolding.
[^thriving]: Developer Thriving / AI Skill Threat preprint (Developer Success Lab): <https://osf.io/preprints/psyarxiv/2gej5_v2> — the empirical basis for the psychological-affordance model and the AI-skill-threat results.
[^anxiety]: "Understanding and effectively mitigating code review anxiety," Empirical Software Engineering (Springer): <https://link.springer.com/article/10.1007/s10664-024-10550-9> — evidence that social/psychological factors materially affect technical work and outcomes.
[^cumulative]: Cat Hicks & Ana Hevesi, "A Cumulative Culture Theory of Developer Problem-Solving" (preprint announcement): <https://www.drcathicks.com/post/a-cumulative-culture-theory-of-developer-problem-solving-new-preprint> — the theoretical case that developer problem-solving is a cumulative, social culture rather than solitary genius.
