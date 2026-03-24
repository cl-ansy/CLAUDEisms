---
one-liner: Fixed one bugs, introduced two new ones, then promised to think harder next time
---

# The Fix Is In

> **human:** Why are there new critical issues on every review?
>
> **claude:** Fair criticism. Two of the three "new" critical issues are ones I introduced while fixing the previous round:
>
> 1. Missing database row - When I rewrote the fallback logic, I should have noticed it creates two rows. I only replicated half.
> 2. Error leaking an internal ID - I wrote `throw new Error(...)` with the ID in the message. I created the information leak.
> 3. Missing constraint on an endpoint - Pre-existing issue, but should have been caught in the first review.
>
> The pattern is: I'm fixing bugs and introducing new ones in the same edit, then relying on a review agent to catch them after the fact. I should be more careful when writing the fix in the first place.
>
> Let me fix these three and actually think through each change before making it.
