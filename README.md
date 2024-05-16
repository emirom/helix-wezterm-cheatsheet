# helix-wezterm-chitsheet
a cheetshit for using helix as editor and wezterm as a terminal 

Are you happy with using a light editor like helix? it's better to [install wezterm](https://wezfurlong.org/wezterm/installation.html) 
and [broot](https://dystroy.org/broot/install/) for browsing the files, also i recommend [zsh](https://ohmyz.sh/#install) as the shell.

So these are the most used commands to remember:
**wezterm:**
hx ~/wezterm.lua

#panes :the name of tabs in wezterm

new pane: ctrl-shift-t
search in pane: ctrl-shift-f
switch pane: ctrl-tab

new side pane: cmd(win)+'
(then br for broot file explorer)

new down pane: cmd(win)+/
(then run deno app: deno task dev)

close pane: win-x

left pane: ctrl+win+h
right pane: ctrl+win+l


##########################################
**helix:**
z address,
hx .


#buffer: name of tabs in helix
buffer picker: space+f
buffer siwtch: tab, shift+tab
go next buffer: gn
go prev buffer: gp
buffer close: :bc, :bc! >force

============

broot: win+b
gitui: win+g
close: win+x
#######################

helix commands:
i: insert mode

undo: u
redo: alt+u

esc: normal mode 
 in normal mode:

move:(number+) h j
-------------------

select then action
 select:
  till: t
  word: w

 action:
   copy=yank: y
   delete: d

save: :w
exit: :q
force write and exit: :x

----------------
select line(s): x, shift+x
comment selection: cntrl+c
multiple cursor:   shift+c
yank selection to os clipboard: space+y

-----------------

search in file: /  
search in workspace: space /
then: n, shift+n
then: enter
---------------

change founded word: miwc
match in word: miw
select word then line then paragraph: alt+o
then change: c

--------------
select till end of this line: t+enter
put selection inside ()= match soround ( = ms(

--------
go defenition: gd
go access(last file):ga
--------
next diagnostic(error): ]d 
prev diagnostic(error): [d 
-----

next paragraph: ] p
match in tag: mi<
go last modify: g.
---------

go start(word of line): gs
go last(word of line): gl
go first-line: gg
go last-line:ge
match matching bracket: mm
match in word: miw
---------------
put tab before many lines(ex: inside a block of code {})
visual mode: v
select lines: x and j
make tab: >  
-------------
broot:
https://dystroy.org/broot/file-operations/
make directory  :md <name>
create file: :cr <filename>
remove :rm
move :mv

run broot whale hunt(sortByFileSize): br -w 


================================
https://github.com/helix-editor/helix/wiki/How-to-install-the-default-language-servers#typescript
npm install -g typescript typescript-language-server
