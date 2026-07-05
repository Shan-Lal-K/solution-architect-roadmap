# 🤝 How We Work Together

This roadmap only works if both of you stay honest about depth over speed. A few ground rules:

## Pace

- **No one moves to Day N+1 until both people have completed Day N's checklist.** If one of you finishes faster, use the extra time to write better interview-question answers, help debug the other's lab, or go deeper on "internal working" — not to rush ahead alone.
- If you're stuck, say so in the issue comments *before* the next session. Two heads on one confusing topic (e.g. SQL Server isolation levels, or K8s networking) beats two people separately confused.

## Workflow per day

1. Whoever is "hosting" that day's session pastes the lesson from Claude into the issue (or links to the chat).
2. Both of you do the lab independently in your own fork/branch, inside `labs/day-XX/`.
3. Open a small PR from your branch with your lab code + filled-in checklist.
4. Review each other's PRs — leave at least one comment (a question, a "nice, but what about X", or a mistake you spot). This is where real learning compounds.
5. Merge, move the card to Done, start the next day.

## Branching

Keep it simple — you don't need GitFlow for a two-person study repo:

```
main            → always the "source of truth", merged & reviewed work
yourname/day-XX → your working branch for that day's lab
```

## Explaining > Copying

If one of you already knows a topic better (e.g. you know .NET/Angular well, your partner might know something else better), **teach it to each other in your own words** in the issue thread before checking the box. Writing your own explanation is what separates "I read about CQRS" from "I could explain CQRS to a review board" — which is the actual goal of this roadmap.

## When you disagree with Claude's answer or with each other

Good — architecture is full of genuine trade-offs, not single right answers. Write down *both* views in the issue with your reasoning. That habit — documenting a decision and its trade-offs — is literally what an Architecture Decision Record (ADR) is, and you'll be doing it for real in the Advanced Track.
