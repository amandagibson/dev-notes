---
sidebar_label: "Co-authored commits"
sidebar_position: 1
---

# Co-authored commits

A co-authored commit credits more than one person for the same change. You add a `Co-authored-by` trailer at the end of the commit message, and GitHub shows every listed author on the commit and counts it toward their contributions.

## Why?

Pair programming, mob sessions, and squashed PRs with several contributors all produce commits that would otherwise credit only one person. Co-authoring keeps the history honest and gives everyone proper credit. It also makes it easier to see who to ask about a piece of code later.

## How?

1. Start a multi-line commit message. Don't type the closing `"` yet. Press Enter and your shell will move to a new line.
2. Leave one blank line between the commit message and the co-author(s).
3. Add one `Co-authored-by:` line per co-author, with no blank lines between them.
4. Type the closing `"` after the last co-author and press Enter.

The format has to be exact, including capitalization and spacing:

```
Co-authored-by: Name Name <githubemail@mail.com>
```

## Example

```bash
git commit -m "Add user authentication

Co-authored-by: Jane Doe <jane@example.com>
Co-authored-by: John Smith <john@example.com>"
```

:::tip[Notes]

For GitHub to credit a co-author, the email must match one tied to their GitHub account.
For privacy-preserving addresses, use `ID+username@users.noreply.github.com`.
:::
