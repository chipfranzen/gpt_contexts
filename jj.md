# Jujutsu (jj) Profile

**Version:** 0.31.0
**OS:** Arch Linux
**Remote:** GitHub
**Main branch bookmark:** `trunk`

## References
- Tutorial: https://jj-vcs.github.io/jj/latest/tutorial/
- Docs: https://jj-vcs.github.io/jj/prerelease/

## Workflow I Use
- **Squash-based workflow**
  1. Create an empty change and give it a description.
  2. Use `jj new` to create a new empty change.
  3. Make edits in the working copy.
  4. Squash changes into the previously described change at `@-`.
- Keep `trunk` as the bookmark for the main branch.
- Use GitHub as remote (`jj git push` / `jj git fetch`).

## Common Commands
- `jj new` → create a new empty change on top of the current one.
- `jj squash` → merge working copy changes into a specified change.
- `jj git push` → push changes to GitHub.
- `jj git fetch` → fetch updates from GitHub.
- `jj log` → view commit history.

## Known Gotchas
- Remember that `jj new` changes the working copy's parent — verify with `jj log` before committing.
- Bookmarks like `trunk` track a specific change, not a branch history in the Git sense.

## Preferred Answer Style
- Assume squash-based workflow above.
- Give explicit `jj` command sequences for any new tasks.
- Clarify how actions affect bookmarks and GitHub remote state.
