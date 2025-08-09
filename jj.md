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
- Use GitHub as remote (`origin`).

## Common Commands
- **Creating and editing changes**
  - `jj new` → create a new empty change on top of the current one.
  - `jj squash` → merge working copy changes into a specified change.
- **Remote setup**
  - `jj git remote add origin git@github.com:<user>/<repo>.git` → add a GitHub remote.
- **Pushing to GitHub**
  - First push of a bookmark:
    ```bash
    jj git push --allow-new
    ```
    (Creates the `trunk@origin` bookmark on the remote.)
  - Subsequent pushes:
    ```bash
    jj git push
    ```
- **Fetching from GitHub**
  - `jj git fetch` → fetch updates from the remote.
- **Viewing history**
  - `jj log` → view commit history.

## Known Gotchas
- `jj git push origin -b trunk` is **not valid** — `jj git push` does not take remote/bookmark as positional arguments.
- First push of a bookmark to a remote requires `--allow-new`.
- Bookmarks like `trunk` track a specific change, not a branch history in the Git sense.

## Preferred Answer Style
- Assume squash-based workflow above.
- Give explicit `jj` command sequences for new tasks.
- Clarify how actions affect bookmarks and GitHub remote state.
