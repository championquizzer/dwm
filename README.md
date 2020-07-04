
# Joydeep's build of Dynamic Window Manager (dwm)
* * *
****About the Project****
* * *
dwm is a dynamic window manager for X developed by suckless.org. It manages windows in tiled, monocle and floating layouts. All of the layouts can be applied dynamically, optimising the environment for the application in use and the task performed.

In tiled layout windows are managed in a master and stacking area. The master area contains the window which currently needs most attention, whereas the stacking area contains all other windows. In monocle layout all windows are maximised to the screen size. In floating layout windows can be resized and moved freely. Dialog windows are always managed floating, regardless of the layout applied.

Windows are grouped by tags. Each window can be tagged with one or multiple tags. Selecting certain tags displays all windows with these tags.

Each screen contains a small status bar which displays all available tags, the layout, the number of visible windows, the title of the focused window, and the text read from the root window name property, if the screen is focused. A floating window is indicated with an empty square and a maximised floating window is indicated with a filled square before the windows title. The selected tags are indicated with a different color. The tags of the focused window are indicated with a filled square in the top left corner. The tags which are applied to one or more windows are indicated with an empty square in the top left corner.
***
****Motivation for the custom build****
***
By default dwm is a barebones window manager and it's meant to be that way! Minimalism is at the core of suckless's philosophy.
I am a heavy desktop user and to use dwm as my window manager I needed some tweaking and tinkering done. This is pretty much adapted to my particular workflow and I have 'patched' some components to the default build.
***
****Patches and features****
***
- [centeredmaster](https://dwm.suckless.org/patches/centeresmaster/) : centers the nmaster area on screen, using mfact * monitor width & height, with the stacked windows distributed to the left and right. It can be selected with [Alt]+[u].
- [fibonnaci](https://dwm.suckless.org/patches/fibonacci/) : new layouts (spiral and dwindle) that arranges all windows in Fibonacci tiles: The first window uses half the screen, the second the half of the remainder, etc. ASCII art and a real screenshot of the spiral arrangement can be seen below.
- [vanitygaps](https://dwm.suckless.org/patches/vanitygaps/) : this patch adds (inner) gaps between client windows and (outer) gaps between windows and the screen edge in a flexible manner. 
- [sticky](https://dwm.suckless.org/patches/sticky/) : A sticky client is visible on all tags.
- [stacker](https://dwm.suckless.org/patches/stacker/) : comprehensive utilities for managing the client stack.
- [real fullscreen](https://dwm.suckless.org/patches/actualfullscreen/) : Actually toggle fullscreen for a window, instead of toggling the status bar and the monocle layout.
