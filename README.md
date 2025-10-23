now im hatdcire progeamer that my current project is:  
  
A terminal emulator idea  
  
I plan make a terminal emulator named tiTTY  
(name could change). writen in pure C. and have scriptible and pluginable structre. It jave few options depending on user usage. if you want core-minimal its just light weight tty. with nto even colors. as you add more things. it grows  
  
like  
  
core-colors  
  
core-image  
  
core-multipaxer  
  
etc.  
apps itself is less then the tty. its just. rgb 0,0,0 bg and rgb 255,255,255 text. nothing more. ignoring evrything else. just i/o and this. not even \x1b[33m would work.  
but what you guys/girls want on your tty so i can add it.  
  
  
---  
  
Core (these are the names listed below):  
  
image: Renders images as text.  
  
inline-image: renderd images inline  
-keybinds: adds keybindings  
  
font: ads font modification instesd drfault fc-match fallback.  
  
color: Handles colors (also lets you change background, foreground, etc.). Normal TTY themes use basic color codes; this adds more flexibility and lets you modify them.  
  
theme: Depends on color and modifies the theme. Essentially, it’s “color on steroids.” It offers a ridiculous amount of options, making even nvim color schemes look basic. Supports up to 32-bit colors (8-bit by default). You can modify tagged sections differently, customize fonts line-by-line, etc.  
  
scripts: Handles scripts.  
  
plugin: Lets you add third-party plugins and provides easier access to core plugins.  
  
bg: Lets you select an image, GIF, or video (even with sound) as the terminal background.  
  
opac: Lets you adjust background opacity.  
  
x11: Adds better configurability with X11.  
  
wayland: Same as X11, but for Wayland.  
  
clip: Clipboard extension.  
  
multioaxer: Tmux, but mine (enhanced version).  
  
tabs: Adds tabs, tab folders, and tab tags.  
  
descriptor-tabs: Depends on tabs. Lets you split the same session in sub-tabs as stdout+stdin, stderr, and optionally stdin separately.  
  
descriptor-multioaxer: Same as descriptor-tabs, but depends on multioaxer instead.  
  
ssh-as-tabs: Depends on tabs and the screen app. Lets you read, write, and monitor connected SSH sessions in new tabs, with the ability to modify their configurations.  
  
hack: Adds nothing (just for fun)  
  
gl46: uses OpenGl 4.6 Core instead OpenGL 3.3 Core.  
  
tty-to-much-yoink: adds so you can use bash or zsh or fish on the go. like first tab has bash second has zsh. nice to have but useless  
  
-vulkan: hijacks rendering and uses vulkan instead gl.  
  
astethics: adds decorstions. not like theme not fow hoe it shows. but what it shows. like does it shows x to close window? does it have minimize button? does it resizable? is it fullscreen etc.  
  
windows: hijacks main logic to fit windows  
  
-mach: windoes but mac  
-bsd: bsd support (lile freebsd)  
  
human-readable: hijacks few outputs. like grep, stat etc. and formats them to more readable way. also supports custom formats  
  
i-want-more-plugins: makes so olugin manager is pluginable  
  
-dweeb: makes a ssh like system. that lets you make a webpage directly shows your terminal and lets ppl use it over web. its a html, js, and css file. so can be encrypted. hosted on local or public. also can select eich commands are blacklisted or whitelisted.  
  
-thats-my-name: prints tits ascii art(not naked). couse name is tiTTY  
  
unit-test: prints stats of ram, gpu,cpu,wm,fans, etc. just QoL  
.  
  
errf: some as human readable but for clang and gcc errors. also shows what the app returned after executing like failed eith -1 or -2 or 5 or sucseded with 0  
  
scrollback: adds scrolback  
  
hot-swap-me: copys scrollback buffer. starts new terminal with bash/zsh or whatever you picked. and forks your process 1 to 1 and kills old one. lets you swap bethwen bash and zsh hot  
  
no-titty-yes-petty: adds digital oet to terminal that you need to feed, play etc. with titty pet feed etc. also games based in nvim keybindings so... probaly better be used to neovim  
  
These are the core plugins.  
  
also kind remendier. non of these are built in. all of thwse are user selected plugins. so somone can have core-dweeb while other dont. its purely plugins. even color and keybinds. without any plugins its black bg white text pty eith nothing  
