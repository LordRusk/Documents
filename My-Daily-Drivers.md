Here are some programs I use on a daily basis:
==============================================
Muh window manager, terminal, file manager, image viewer, text editor... everything.

Window manager | dwm
--------------------
dwm[0] is my window manager of choice, you here can find my personal fork[1] on my github.
What differences does dwm have to other, similar, window managers?  
  - Abstract Logic of Stacking: Unlike other window managers such as i3[2], dwm treats windows in a stack, with a master window and slave windows. The logic here is that, the newest window you open, should take up the most screen realestate. It's like adding a new peice of paper to a stack of papers. This allows for very customizable layouts, and they can be very easily implemented because they all follow this abstract logic. Some notable ones to checkout are fibobacci[3] and centered master.[4]
  - There is no config file, persay. There is, but a lot can go wrong with a live config file like i3 has, if you mess something up, it breaks. That is why dwm doesn't have such a file, only a config.h file read at installation. This means that all changes you make, don't cause any error and nothing about the windowmanager can be effected after it is compiled, Making it safe and prone to less bugs. You may think it would be boring having to recompile every time you make a change, but you are using linux people. I have (n)vim set to auto compile whenever I save config.h or config.def.h files. It's that easy.
  - It is fast and small. It is under 5000 sloc and coded in C, it's going to be fast and reliable.

Terminal | st
-------------
st[5] is the simple(suckless) terminal. you can find my personal fork[6] on my github.
What differences does st have compaired to other terminals?
  - Efficency. xterm[7] is 65K lines of code, rxvt[8] is a smaller at 32k lines of code, but, WHY SO MANY LINES? Why do terminal emulators have to be so bloated? sure xterm can emulate obscure and obsolete terminals you will never need[9]. but rxvt has no exuses. All it is is bloat, plain and simple. st is a prime example of why terminals do not need so many lines of code, currently st has ~2650 lines of code. and currently supports:
    - most VT10X escape sequences
    - serial line support
    - XIM support
    - utmp via utmp(1)
    - clipboard handling
    - mouse and keyboard shortcuts (via config.h)
    - UTF-8
    - wide-character support
    - resize
    - 256 colors and true colors
    - antialiased fonts (using fontconfig)
    - fallback fonts
    - line drawing
  
  And anything else you might want, like transparency, can be easily added through patches.[10] Anyone who thinks 32k or 65k lines of code is acceptable for a terminal emulator, should proboby switch to windows, because that type of bloat does not belong in the linux community.

Browser | surf
--------------
surf[11] is the suckless browser. It is built with webkit2gtk and gtk(3)+. You can find my personal fork[12] on my github.
  - Why surf and not, firefox or chromium? Because they are bloated and centrolised. Everything I want out of a browser surf has, or I have added to it. Who needs built in search bar taking up screen realestate when you can use dmenu[13]? Why have built in tabs when you can just use tabbed[14]? Why watch youtube videos in browser when you can get better quality and no ads by playing it exterally through mpv[15]? Want bookmarks? make a simple script with dmenu and boom. Browsers don't have to be so bloated or so centrolised.

File Manager | lf
-----------------
lf[16] stands for list file, and is a very fast, minimalist, scriptable terminal file manager. You can find my lfrc in my dotfiles[17].
- lf has the great layout of ranger, but isn't coded in python, meaning it has the speed of vifm, but doesn't look like a retarded three legged cat on xanex, and is heavily scriptable and can molded into the perfect file browser for you.
  - Why a terminal file manager and not a gui file manager? If you think that a gui is needed for something as simple as a file manager, then you should probably go back to ubuntu. Better yet, just go back to windows, we don't need that type of mentality in the linux community. Maybe take a look at this[18] on your way out.
