---
name: entry
description: Create a new CLAUDEisms journal entry from a pasted chat snippet. Use when the user says "entry", "log this", "add this gaffe", or pastes a Claude chat excerpt to document.
---

Create a new CLAUDEisms journal entry from this chat snippet:

$ARGUMENTS

Steps:

1. Read the chat snippet and identify the gaffe, poor decision, or amusing behavior Claude exhibited.
2. Pick a short, punchy title that captures the humor (e.g., "The Phantom Import", "Confidently Wrong About Its Own Name").
3. Check the `_entries/` directory for existing files to determine the next entry number and confirm the naming convention.
4. Create a new markdown file at `_entries/NNNN-kebab-case-title.md` using this format:

```markdown
---
title: <Title>
one-liner: <A short, punchy summary of the gaffe for the README table. One sentence fragment, no period. If the value contains quotes or special YAML characters (:, #, etc.), wrap it in single quotes.>
---

> **human:** message here
>
> **claude:** response here
>
> **human:** follow-up here
```

Do NOT include a `# Title` heading in the content - the layout renders the title from frontmatter.

Format the chat to resemble a real Claude Code terminal session. Use `**human:**` and `**claude:**` as speaker prefixes (lowercase, bold). Each speaker turn is a blockquote line. Separate turns with a blank blockquote line (`>`). Trim to just the funny/relevant part.

5. Redact any user-specific or project-specific information from the chat before writing. Replace real project names, file paths, variable names, team names, or other identifying details with generic placeholders (e.g., "the project", "the service", "TICKET-123") while preserving the chat structure, intent, and humor. The entry should be funny to anyone without revealing what the user was working on.
6. Keep the tone lighthearted and fun per the repo's guidelines.
7. Show the user the created file path and a one-line summary of the entry.
