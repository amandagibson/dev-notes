---
sidebar_label: "Co-author commits"
sidebar_position: 1
---

# How to co-author commits:

## Steps

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
