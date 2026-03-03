## Input vs. Output Metrics

Look, we've all been in that meeting where someone says "we need more PRs!" like they're ordering widgets from a factory. This is for those conversations, when you need to explain why measuring developer productivity isn't like counting hamburgers flipped per hour, and why your engineering team will absolutely game any metric you give them (because they're smart, and that's literally what you pay them to do).

In system design, there's a critical distinction between what goes into a system and what comes out:
- Input metrics: what you control, the work you do
- Output metrics: the result, what actually happens

Optimizing inputs doesn't guarantee good outputs. In fact, it often backfires.

### The developer productivity parallel

| Dimension | Input Metric | Output Metric | What's Wrong |
|-----------|--------------|---------------|--------------|
| Code Shipping | Lines of code written | Business value delivered | Optimizing LOC creates bloat |
| Pull Requests | Number of PRs created | Impact of those PRs | More PRs isn't better features |
| Commits | Commit frequency | Working software | Frequent commits isn't progress |
| Hours Worked | Time at desk | Quality of output | Long hours isn't productivity |
| Meetings Attended | Number of meetings | Decisions made | More meetings isn't better decisions |

### The problem: optimizing outputs as inputs

When you say "we want more PRs per week," here's what happens:

Teams respond by creating more, smaller PRs. They split logical changes across multiple PRs. They merge low-quality code faster. They skip code review rigor.

Result: high throughput, low quality, low impact.

### The solution: frame outputs as desired outcomes

**Wrong (input framing):**
> "We want to increase PR throughput. Teams should be merging more PRs per week."

Result: teams game it by creating trivial PRs.

**Right (output framing):**
> "We want to reduce friction and increase flow through the system. Faster code reviews and deployments make your life better."

Result: teams focus on removing blockers and shipping meaningful work.

### The chain of causation

```
Input -> Process -> Output -> Outcome
Work     Tools     Speed     Value
Done     Quality   Quality   Shipped
```

We often measure work done (input) and assume it correlates with value (outcome). The correlation is weak without controlling for quality.

```
Input:   10 developers wrote code
Output:  50 PRs merged this week
Outcome: We shipped 1 bug-ridden feature

vs.

Input:   10 developers focused on 1 critical feature
Output:  5 PRs merged after thorough review
Outcome: We shipped 1 solid feature customers love
```

The output numbers look worse, but the outcome is better.

### What to measure instead

**Input metrics (what we control):**
- Code quality standards applied
- Testing coverage written
- Design review completion
- Architectural decisions made
- Security scanning run

**Output metrics (what actually happens):**
- Features deployed
- Defects found in production
- User engagement metrics
- Performance improvements
- Customer satisfaction

**Outcome metrics (the real goal):**
- Revenue impact
- User adoption
- System reliability
- Developer satisfaction
- Time-to-value

### Common mistakes

**Lines of code:**
Wrong: "Developers wrote 10,000 lines of code."
Right: "We deleted 2,000 lines of legacy code and improved maintainability."

**Meeting attendance:**
Wrong: "100% of developers attended standup."
Right: "Teams feel aligned and unblocked."

**Commit frequency:**
Wrong: "Developers averaged 5 commits per day."
Right: "Code changes are reviewed and tested before merging."

**Story points:**
Wrong: "Team completed 50 story points this sprint."
Right: "Team delivered features that users are actually using."

### The mental shift

Common leadership thinking: if developers work harder (input), they'll be more productive (output).

Reality: if we remove friction and improve flow (output), developers will naturally do better work.

- Input focus pushes harder on developers. This leads to burnout, gaming, and quality drops.
- Output focus improves the system. This is sustainable and quality-driven.

## Using this framework

**When someone says "we need more PRs per week":**
> "That's an input target. Let's think about outputs instead: do we want faster code reviews? Fewer blockers? Better collaboration? Those are outputs. Increased PR count might happen as a side effect, but it's not the goal."

**When setting OKRs:**
> "Let's frame this as an output: 'Reduce time from code review to production,' instead of an input: 'Merge 20% more PRs.'"

**When defending qualitative work:**
> "Code refactoring isn't measured as an output (PRs merged), but it's critical output (technical debt reduction). Some of our most valuable work doesn't look like high throughput."

**When explaining to executives:**
> "Think of a restaurant. The input is: how long does a chef spend cooking? The output is: how many meals served? The outcome is: how many customers come back? We want to optimize outcome, which requires managing outputs, not just maximizing inputs."

## Related

- Goodhart's Law: when you measure the wrong thing, it stops being useful
- Leading vs. Lagging Indicators: inputs are leading, outcomes are lagging
- DORA Metrics: output-focused (deployment frequency, lead time) vs. outcome-focused (system stability)
- [Cycling Analogy](cycle-time.md): cadence as an output metric
- [Health Analogies](health.md): healthy ranges vs. targets to minimize
