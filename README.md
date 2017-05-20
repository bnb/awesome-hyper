# PopClip/Alfred for Hyper Terminal

I tried to find a way to use this elegant terminal with **[Alfred](https://www.alfredapp.com)** and **[PopClip](http://pilotmoon.com/popclip/)** to implement quick actions. In which case, you can quickly run a command from anywhere at ease.

However, Hyper is built based on **Node.js** using [Electron](https://electron.atom.io) which does not come with AppleScript support.

So I took a detour, utilizing an alternative.

## Result

- #### [PopClip Extension](http://pilotmoon.com/popclip/)

![popcliptest](https://github.com/fuchenxu2008/Hyper-PopClip-Alfred-Extension/raw/master/PopClip/PopCliptest.gif)

- #### [Alfred](https://www.alfredapp.com)

![alfredresult](https://github.com/fuchenxu2008/Hyper-PopClip-Alfred-Extension/raw/master/Alfred/alfredtest.gif)

## Principle

- #### [PopClip](http://pilotmoon.com/popclip/)

1. It first copys the text you select to the **ClipBoard**.

2. Then it activates the Hyper App and brings it to front, launching it if it is not open.

3. Considering the lauching speed, delay **1 second** (May change for different computers) to wait for the window popping up.

4. Simulate the keypress combo **⌘+V** to perform **Paste**.

5. Delay for 0.5 seconds (Optional) and simulate keypress **Return**.

- #### [Alfred](https://www.alfredapp.com)

 Similar as above, the AppleScript code is altered accordingly.

![Alfred](https://github.com/fuchenxu2008/Hyper-PopClip-Alfred-Extension/raw/master/Alfred/Alfred.png)

## Install

Install [PopClip Extension](https://github.com/fuchenxu2008/Hyper-PopClip-Alfred-Extension/raw/master/PopClip/Hyper.zip) here and rename the zip file to **"Hyper.popclipext"**.

Install [Alfred AppleScript](https://github.com/fuchenxu2008/Hyper-PopClip-Alfred-Extension/raw/master/Alfred/HyperAlfred.applescript) here and put the content text to Alfred Terminal Settings section.



[Link to my original repository](https://github.com/fuchenxu2008/Hyper-PopClip-Alfred-Extension)
