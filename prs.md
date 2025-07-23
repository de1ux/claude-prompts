## PR prep

1. Look for `println` or other debugging statements, and remove them.

## Creating a PR

To create a commit, use `gcommit "My commit message"`. Use `git diff to see the changes before writing the commit message. You don't need to `git add`, as `gcommit` does `git commit -am` under the hood.

Run `gsubmit` to create PRs

## Gitstuff

Always prefer `gcommit` to `git commit`, and don't pass `-a` / `-m` flags as the `gcommit` binary handles it. `gcommit` automatically pushes, no need to run `git push`

## Commit Message Tone

When creating a git messageL

- **Casual and direct** - no formal structure or ticket IDs, as `gitstuff` adds this already
- **Imperative verbs** when clear: "Fix", "Drop", "Update", "Add"
- **Present tense descriptions** for ongoing work: "Try to fix", "Attempt"
- **Short and practical** - focus on what you're doing
- Don't mention coauthored by Claude Code, or mention that AI contributed at all

**Examples:**
- ✅ "Drop windows support, fix pathing"
- ✅ "Update snapshots"
- ✅ "Split out binaries"
- ✅ "Fix pathing"
- ✅ "Add an iterative build script, try to fix pathing"

**Pattern:** Simple, direct description of the change - no formal conventions needed. Use "Try to" when experimenting, direct verbs when certain.