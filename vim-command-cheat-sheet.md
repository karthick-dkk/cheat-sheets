# 📝 Vim Complete Advanced Command Cheat Sheet

A quick and practical Vim reference you can use daily.

---

## 🔁 Modes

| Key | Action |
|----|------|
| `i` | Insert mode |
| `I` | Insert at beginning of line |
| `a` | Append after cursor |
| `A` | Append at end of line |
| `o` | Open new line below |
| `O` | Open new line above |
| `Esc` | Back to Normal mode |
| `v` | Visual mode |
| `V` | Visual line mode |
| `Ctrl+v` | Visual block mode |
| `:` | Command mode |

---

## 📁 File Operations

| Command | Action |
|------|------|
| `:e filename` | Open a file |
| `:e scp://user@host//path/file` | Open remote file via SSH |
| `:w` | Save file |
| `:q` | Quit Vim |
| `:wq` or `:x` | Save and quit |
| `:q!` | Quit without saving |
| `:qa!` | Quit all without saving |
| `:mksession my.vim` | Save session |
| `:source my.vim` | Load session |

---

## 🧭 Navigation

| Key | Action |
|----|------|
| `h / l` | Move left / right |
| `j / k` | Move down / up |
| `w / e` | Next word / end of word |
| `b` | Previous word |
| `0` | Start of line |
| `$` | End of line |
| `gg` | Top of file |
| `G` | Bottom of file |
| `5G` or `:5` | Go to line 5 |
| `H / M / L` | Top / Middle / Bottom of screen |
| `{ / }` | Previous / Next paragraph |
| `Ctrl+d / Ctrl+u` | Half page down / up |
| `Ctrl+f / Ctrl+b` | Page forward / backward |
| `%` | Jump to matching bracket |
| `Ctrl+o / Ctrl+i` | Older / newer cursor position |

---

## ✏️ Editing

| Key | Action |
|----|------|
| `x` | Delete character |
| `dd / ndd` | Delete line / n lines |
| `yy / nyy` | Copy line / n lines |
| `p / P` | Paste after / before cursor |
| `xp` | Swap characters |
| `r<char>` | Replace one character |
| `R` | Replace mode |
| `u` | Undo |
| `Ctrl+r` | Redo |
| `.` | Repeat last command |
| `>> / <<` | Indent / Un-indent |
| `J` | Join line |
| `ggVGy` | Copy entire file |
| `ggVGd` | Delete entire file |
| `ggVGJ` | Join all lines |
| `gg=G` | Auto-indent file |
| `ggVGgU` | Uppercase entire file |

---

## 🔍 Search & Replace

| Command | Action |
|------|------|
| `/word` | Search forward |
| `?word` | Search backward |
| `n / N` | Next / Previous match |
| `:%s/foo/bar/g` | Replace all |
| `:%s/foo/bar/gc` | Replace with confirm |
| `:1,10s/foo/bar/g` | Replace lines 1–10 |
| `:.,$s/foo/bar/g` | Replace current to end |

---

## 🎯 Visual Mode Tricks

| Key | Action |
|----|------|
| `> / <` | Indent / Un-indent |
| `y / d` | Copy / Delete selection |
| `~` | Toggle case |
| `I text` | Insert text at start |
| `A text` | Append text at end |

---

## 🧩 Buffers, Splits & Tabs

| Command | Action |
|------|------|
| `:split file` | Horizontal split |
| `:vsplit file` | Vertical split |
| `Ctrl+w h/j/k/l` | Move between splits |
| `Ctrl+w w` | Cycle splits |
| `:tabnew file` | New tab |
| `gt / gT` | Next / Previous tab |
| `:ls` | List buffers |
| `:b1 / :b#` | Switch buffer |
| `:bnext / :bprev` | Next / Previous buffer |
| `:bd` | Close buffer |

---

## 🎬 Macros & Registers

| Command | Action |
|------|------|
| `qa` | Record macro in register a |
| `q` | Stop recording |
| `@a` | Run macro |
| `@@` | Repeat macro |
| `:reg` | Show registers |
| `"ayy / "ap` | Yank / Paste using register |
| `ma / \`a` | Set / Jump to mark |
| `:%y+` | Copy file to system clipboard |
| `"+p` | Paste from system clipboard |

---

## 💻 Command Line Tricks

| Command | Action |
|------|------|
| `:!ls` | Run shell command |
| `:!python file.py` | Run Python script |
| `Ctrl+z` | Suspend Vim |
| `fg` | Resume Vim |

---

## ⚙️ Useful `.vimrc` Settings

```vim
set number
set relativenumber
set autoindent
set smartcase
set ignorecase
syntax on
set paste
set nopaste
