## 1. Cursor Navigation

| Shortcut | Action |
|---|---|
| `Ctrl + A` | Move cursor to beginning of line |
| `Ctrl + E` | Move cursor to end of line |
| `Ctrl + B` | Move cursor one character left |
| `Ctrl + F` | Move cursor one character right |
| `Alt + B` | Move cursor one word backwards |
| `Alt + F` | Move cursor one word forwards |

## 2. Command History

| Shortcut | Action |
|---|---|
| `Ctrl + P` | Display previous command |
| `Ctrl + N` | Display next command |
| `Ctrl + R` | Search command history backwards |
| `Ctrl + G` | Cancel history search |
| `Up Arrow` | Display previous command |
| `Down Arrow` | Display next command |

## 3. Deleting Text

| Shortcut | Action |
|---|---|
| `Ctrl + W` | Delete previous word |
| `Ctrl + U` | Delete from cursor to beginning of line |
| `Ctrl + K` | Delete from cursor to end of line |
| `Ctrl + H` | Delete character before cursor |
| `Ctrl + D` | Delete character under cursor |

## 4. Restoring and Manipulating Text

| Shortcut | Action |
|---|---|
| `Ctrl + Y` | Restore previously deleted text |
| `Ctrl + T` | Swap two characters before cursor |
| `Alt + T` | Swap two words before cursor |
| `Ctrl + _` | Undo previous editing action |

## 5. Terminal Controls

| Shortcut | Action |
|---|---|
| `Ctrl + L` | Clear terminal screen |
| `Ctrl + C` | Interrupt foreground process |
| `Ctrl + Z` | Suspend foreground process |
| `Ctrl + D` | Send EOF; normally exits Bash on an empty command line |

## Notes

- These shortcuts primarily apply to Bash Readline in Emacs-style editing mode.
- `Ctrl + C` interrupts a foreground process; `Ctrl + Z` suspends it.
- `Ctrl + D` has context-dependent behaviour.
- `Ctrl + R` is useful for searching previously executed commands.
- `Ctrl + U`, `Ctrl + K` and `Ctrl + Y` help edit long commands without retyping them.