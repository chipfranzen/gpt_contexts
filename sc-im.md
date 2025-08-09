**Version:** 0.8.5
**OS:** Arch Linux (default terminal, no tmux)
**Keybindings:** Default (no ~/.scimrc customizations)

## References
- Cheat sheet: https://cheatography.com/isaacnewton/cheat-sheets/sc-im/
- Tutorial: https://github.com/jonnieey/Sc-im-Tutorial

## Behaviors I Rely On
- **Labels (text) from normal mode:**
  - `<text` → left-aligned
  - `\text` → centered
  - `>text` → right-aligned
- **Values / formulas:**
  - `=123`
  - `=A1+5`
  - `="foo"`
- **Row / column ops:**
  - `ic` → insert column to left
  - `oc` → insert column after
  - `ir` → insert row above
  - `or` → insert row below
  - `dc` / `dr` → delete column/row

## Known Gotchas
- `i` is not insert by default
- Strings must be quoted if entered in value/formula mode
- Typing letters first in edit mode won’t work unless using label prefix `<`, `>`, or `\`

## Preferred Answer Style
- Assume default bindings above
- Prefer referencing cheat sheet for confirmation
- Give exact key sequence for normal mode where possible
