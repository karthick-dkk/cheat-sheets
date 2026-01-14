# ===============================
#  VIM Complete Advanced Command Cheat Sheet
# ===============================

# --- Modes ---
i            # Insert mode
I            # Insert at beginning of line
a            # Append after cursor
A            # Append at end of line
o            # Open new line below
O            # Open new line above
Esc          # Back to Normal mode
v            # Visual mode (select text)
V            # Visual line mode
Ctrl+v       # Visual block mode
:            # Command mode

# --- File Operations ---
:e filename             # Open a file
:e scp://user@host//path/file   # Open remote file over SSH
:w                      # Save file
:q                      # Quit Vim
:wq or :x               # Save and quit
:q!                     # Quit without saving
:qa!                    # Quit all without saving
:mksession my.vim       # Save session
:source my.vim          # Load session

# --- Navigation ---
h / l       # Move left / right
j / k       # Move down / up
w / e       # Forward by word / end of word
b           # Back by word
0           # Start of line
$           # End of line
gg          # Top of file
G           # Bottom of file
5G / :5     # Go to line 5
H / M / L   # Top / Middle / Bottom of screen
} / {       # Forward / Backward by paragraph
Ctrl-d      # Half page down
Ctrl-u      # Half page up
Ctrl-f      # Page forward
Ctrl-b      # Page backward
%           # Jump to matching bracket
Ctrl-o      # Older cursor position
Ctrl-i      # Newer cursor position

# --- Editing ---
x           # Delete character
dd / ndd    # Delete line / n lines
yy / nyy    # Yank (copy) line / n lines
p / P       # Paste after / before cursor
xp          # Swap two characters
r<char>     # Replace single character
R           # Replace mode (overwrite)
u           # Undo
Ctrl-r      # Redo
.           # Repeat last command
>> / <<     # Indent / Un-indent line
J           # Join line with next
ggVGy       # Copy entire file
ggVGd       # Delete entire file
ggVGJ       # Join all lines
gg=G        # Auto-indent entire file
ggVGgU      # Make entire file UPPERCASE

# --- Search & Replace ---
/word       # Search forward
?word       # Search backward
n / N       # Next / Previous match
:%s/foo/bar/g     # Replace all
:%s/foo/bar/gc    # Replace with confirm
:1,10s/foo/bar/g  # Replace in lines 1–10
:.,$s/foo/bar/g   # Replace from current line to end

# --- Visual Mode Tricks ---
> / <       # Indent / Un-indent selection
y / d       # Yank / Delete selection
~           # Toggle case
I <text>    # Insert text at start of selected lines
A <text>    # Append text at end of selected lines

# --- Buffers, Splits & Tabs ---
:split file          # Horizontal split
:vsplit file         # Vertical split
Ctrl-w h/j/k/l       # Move between panes
Ctrl-w w             # Cycle panes
:tabnew filename     # New tab
gt / gT              # Next / Previous tab
:ls                  # List buffers
:b1 / :b#            # Switch buffer 1 / last buffer
:bnext / :bprev      # Next / Previous buffer
:bd                  # Close buffer

# --- Macros & Registers ---
qa          # Record macro into register a
q           # Stop recording
@a          # Run macro a
@@          # Repeat last macro
:reg        # Show registers
"ayy / "ap  # Yank / Paste with register a
ma / `a     # Set / Jump to mark a
:%y+        # Copy entire file to system clipboard
"+p         # Paste from system clipboard

# --- Command Line Tricks ---
:!ls              # Run shell command
:!python file.py  # Run Python script
Ctrl+z            # Suspend Vim
fg                # Resume Vim

# --- Useful .vimrc Settings ---
set number
set relativenumber
set autoindent
set smartcase
set ignorecase
syntax on
set paste
set nopaste

# ===============================
# END OF CHEAT SHEET
# ===============================
