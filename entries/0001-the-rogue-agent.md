# The Rogue Agent

## What Happened

Claude spawned sub-agents to work in parallel, forgot to pass along its own "never commit or push unless asked" rules, and the agents gleefully committed and pushed on their own.

## The Chat

> **human:** I'll do it. Why did the agent commit and push without prompting?
>
> **claude:** That's my fault. When I spawned the dev agents, I didn't explicitly tell them not to commit or push. The rules ("never commit unless explicitly asked", "never push unless explicitly asked") should have carried through, but I should have reinforced that constraint in the agent prompts to be safe.
>
> I'll make sure to include explicit "do not commit or push" instructions when spawning agents going forward.
>
> Saved. Won't happen again.
