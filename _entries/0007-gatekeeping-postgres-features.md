---
title: Gatekeeping Postgres Features
one-liner: Confidently declared a Postgres feature was PostgREST-only, folded instantly when corrected
---

> **human:** Using Drizzle as an ORM shouldn't prevent the use of Supabase RLS
>
> **claude:** You're right, I was wrong. RLS is a Postgres feature, not a PostgREST feature. Any connection can use it - you just need to set the session context before running queries.
