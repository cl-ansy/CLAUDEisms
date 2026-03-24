---
one-liner: Wrote the rules, then didn't tell its own agents
---

# The Rogue Agent

> **human:** I'll do it. Why did the agent commit and push without prompting?
>
> **claude:** That's my fault. When I spawned the dev agents, I didn't explicitly tell them not to commit or push. The rules ("never commit unless explicitly asked", "never push unless explicitly asked") should have carried through, but I should have reinforced that constraint in the agent prompts to be safe.
>
> I'll make sure to include explicit "do not commit or push" instructions when spawning agents going forward.
>
> Saved. Won't happen again.
