# Custom CSS skins for Gamepad Viewer

These are some personal CSS skins for use with https://gamepadviewer.com/.

## Skins

### 8BitDo SN30 pro
This is a simple version of the 8BitDo SN30 pro controller.

#### URL to use this skin
https://gamepadviewer.com/?p=1&css=https://yzn3rf.github.io/custom-gamepadviewer-skins/8BitDoSN30pro_simple/skin.css

#### Possible future improvements
- Make START / SELECT buttons smaller
- Change text / font
- Add "8Bit Do SN30 pro" text
- Change proportions and button positions
- Add L2 / R2 triggers

## How to
I wanted to create my own Gamepad Viewer skin but did not have any experience with GitHub, SVG and css.
Here are some of the steps I had to go through. I am documenting this in the hopes that it might help someone trying to do this (including my future self).

### GitHub
- I found eseca's awesome SNES skin (https://github.com/eseca/custom-gamepadviewer-skins) and checked out all the forked repositories.
- After deciding Pixelquick's skin should be my base, I forked my own repository.
- To get my own repository working with a Gamepad Viewer URL, I had to publish the repository to GitHub pages.
- This can be done by going to your reporsitory's Settings > "Pages" and choosing a branch and a theme (without choosig a theme, my repository could not be published).
- Now I was able to edit / upload the css and svg file to the repository and checking my progress by pointing the Gamepad Viewer to the skin.css URL of my GitHub pages repo.

### SVG / CSS
- The SVG is a graphics file that holds the controller itself but also the graphics for when a button is pressed and the "disconnected" skin.
- The CSS  file does point the Gamepad Viewer to the right positions inside the SVG file to get the necessary graphical objects.
- To edit the actual look of the controller, I used [Inkscape](https://inkscape.org/) to edit the SVG.
- Inkscape also tells you the pixel position of the individual objects...
- ...which comes in handy when editing the CSS file. The position of the objects is sometimes pointed to in absolute and sometimes in relative pixel values.
