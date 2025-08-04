# VIM FU

### Basic Use
```
<Esc> is the escape key or use <ctrl>[  sometimes written as  <C-[>

vimtutor    : starts vim editing a copy of a tutorial file -- very good.
i           : insert mode. Next keys typed are inserted into the file.
<Esc>       : Escape from insert mode so you can navigate and use edit commands (stop selecting)
h j k l     : move cursor ( h: ←  j: ↓  k: ↑  l: → )
A           : Append at end of line
o           : Insert at new line below
u           : undo last command, again and again
x           : delete character under cursor
dw          : delete everything right from the cursor to the start of next word (and put it into the default register)
dd          : delete line (and put it into the default register)
p           : paste the default register

/myname     : search forward for myname

:wq         : write and quit
:x          : write and quit
:w filename : write a copy of the file you are editing as filename
:q!         : quit without saving even if changes were made!
:help       : display help
<Tab>       : use tab completion to scroll through commands that start with what you typed

# COPY PASTE  (for CUTting lines use dd as described above)
v           : visual mode -- use to select text with cursor movement or mouse
y           : use to yank (copy) what was selected
<Esc>       : esc gets you back to the main mode
p           : put (paste)

^ w e $     : bigger movements: beginning of line, word, end of word, end of line

# Modes:
 normal, insert and visual, there are others too
 <Esc>    takes you back to normal

# Enter a number before a command to repeat it, examples:
   10w      : skip forward 10 words
   10dd     : delete 10 lines

# Commands are case sensitive:
   c        : starts a change command
   C        : change to end of line (same as c$)
   ce       : change to end of word (a complete change command)
```



### find and replace 
```
:%s/<SEARCH_TERM>/<REPLACE_TERM>/g
```




## freeze the top 10 lines (keep them always visable)
```
:split
:resize 10
gg
Ctrl-w w
```