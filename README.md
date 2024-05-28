# helix-wezterm-cheatsheet
a cheetshit for using helix as editor and wezterm as a terminal 

Are you happy with using a light editor like helix? <br />
It's better to [install wezterm](https://wezfurlong.org/wezterm/installation.html) 
and [broot](https://dystroy.org/broot/install/) for browsing the files, also i recommend [fish](https://fishshell.com/) as the shell. <br />
<br />
So these are the most used commands to remember:<br />
**wezterm:**<br />

hx ~/wezterm.lua <br />

#panes :the name of tabs in wezterm <br />

new pane: ctrl-shift-t <br />
search in pane: ctrl-shift-f <br />
switch pane: ctrl-tab <br />

new side pane: cmd(win)+' <br />
(then br for broot file explorer) <br />

new down pane: cmd(win)+/ <br />
(then run deno app: deno task dev) <br />

close pane: win-x <br /
left pane: ctrl+win+h <br />
right pane: ctrl+win+l <br />

-------------

**helix:**

z address<br />
hx . <br />

-------------
<br />

#buffer: name of tabs in helix <br />
buffer picker: space+f <br />
buffer siwtch: tab, shift+tab <br />
go next buffer: gn <br />
go prev buffer: gp <br />
buffer close: :bc, :bc! >force <br />

-------------- 
broot: win+b <br />
gitui: win+g <br />
close: win+x <br />

--------------
helix commands: <br />
i: insert mode <br />
esc: back to normal mode <br />

undo: u <br />
redo: alt+u <br />

esc: normal mode  <br />
 in normal mode: <br />
ove:(number+) h j <br />

------------------
select then action <br />
 select: <br />
  till: t <br />
  word: w  <br />

 action: <br />
   copy=yank: y <br />
   delete: d <br />

save: :w <br />
exit: :q <br />
force write and exit: :x <br />

-------------
select line(s): x, shift+x <br />
<br />
select all of the page:<br />
go first line: gg <br />
visual mode: v <br />
go end: ge <br />
yank : y <br />
<br />
yank selection to os clipboard: space+y <br />
comment selection: cntrl+c <br />
multiple cursor:   shift+c <br />


-------------

search in file: /  <br /
search in workspace: space /  <br /
next result: then: n, <br />
prevois result: shift+n <br />
move cursor to founded result: enter <br />

-------------

change founded word: miwc <br />
match in word: miw <br />
select word then line then paragraph: alt+o <br />
then change: c <br />

--------------
<br />
select till end of this line: t+enter <br />

put selection inside ()= match soround ( = ms(  <br />

--------

go defenition: gd <br />
go access(last file):ga <br />

--------
next diagnostic(error): ]d <br />
prev diagnostic(error): [d <br />

-----

next paragraph: ] p <br />
match in tag: mi<   <br />
go last modify: g. <br />

-------------

go start(word of line): gs <br />
go last(word of line): gl <br />
go first-line: gg <br />
go last-line:ge <br />
match matching bracket: mm <br />
match in word: miw <br />

-------------

put tab before many lines(ex: inside a block of code {}) <br />
visual mode: v <br />
select lines: x and j <br />
make tab: >  <br />


fix ts-lsp in helix:
https://github.com/helix-editor/helix/wiki/How-to-install-the-default-language-servers#typescript <br />
npm install -g typescript typescript-language-server

-------------
replace all : <br />
select a word: w <br />
put to register: @ <br />
visual mode: v <br />
find next: n <br />
change word: c <br />
type your word

-------------
**broot:**

https://dystroy.org/broot/file-operations/

make directory  :md <name> <br />
create file: :cr <filename> <br />
remove :rm <br />
move :mv <br />

run broot whale hunt(sortByFileSize): br -w <br /> 


