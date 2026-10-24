---
sidebar_label: "Protected branches"
sidebar_position: 2
---

# Protected Branches

A protected branch is a branch (usually main or production) with rules that restrict how changes can reach it. Typical rules include:

- **No direct pushes.** Changes have to come in through a pull request.
- **Required reviews.** At least one teammate must approve before merging.
- **No force pushes or deletion.** History can’t be rewritten and the branch can’t be removed by accident.
- **Required status checks.** Tests, linting, and builds must pass first.

## Why?

Your main branch is the source of truth and protection keeps untested or unreviewed code out of it. In a team it also builds in code review as a habit rather than something people have to remember. Everyone works the same way, so one person’s mistake doesn’t land on everyone else, and there’s a clear history of who approved what.

Rule of thumb: protect any branch you’d be unhappy to see broken, and turn on rules for admins as well, since “just this once” is how most accidents happen.

## How?

1. Open the repository and click Settings.
2. In the left menu, click Branches.
3. Next to “Branch protection rules,” click Add rule.
4. Under “Branch name pattern,” enter the branch to protect (e.g. `main`). Patterns work too, so `release/*` covers every branch starting with `release/`.

5. Choose your rules. A sensible baseline for a team are:

- Require a pull request before merging, with at least one approval
- Require linear history, if your team prefers rebasing or squashing
- Leave force pushes and deletions off

6. Click create.

:::tip[Notes]

You need admin permissions on the repository in order to create and apply these protection rules!
:::
