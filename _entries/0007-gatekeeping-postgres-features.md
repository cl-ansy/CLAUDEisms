---
title: Gatekeeping Postgres Features
one-liner: Confidently attributed a core Postgres feature to PostgREST, then immediately folded when corrected
---

> **human:** Using an ORM shouldn't prevent the use of row-level security
>
> **claude:** You're right, I was wrong. RLS is a Postgres feature, not a PostgREST feature. Any connection can use it - you just need to set the session context before running queries.
