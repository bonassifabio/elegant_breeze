Dependencies
==============
* qtcurve
* KDE 4.13 or higher (not tested for previous versions)

Installation
==============
Patched QtCurve
------
I've patched QtCurve to remove the shadows of popup-menus and tooltips. Yep, actually QtCurve doesn't allow to change them. I plan to add an option and submit a pull request, but it will take some time. In the meanwile, you can clone [my fork QtCurve](https://github.com/gnufabio/qtcurve) and use it instead of the packaged QtCurve. Give a look to it for more details.

Install theme
------
### Using Script
1. Download a copy of the current master
2. Unpack it
3. Execute the 'install' bash script
4. Open System Settings and choose the new theme both in Workspace Appearance and in Application Appearance
5. Enjoy :)

The script may not find your KDE directory. If so, you have to install the theme manually.

### Manually
1. Download a copy of the current master tree. (Or download a version tag from Releases page)

2. Unpack it. For conviniente, i will call the directory in which you unpack it $DIR. (e.g. `$DIR=~/Desktop/ElegantBreeze`)

3. Install the **Aurora Theme**. To do so, from bash: `cp -r ${DIR}/Aurorae_theme/ElegantBreeze ~/.kde4/share/apps/aurorae/themes/ElegantBreeze` (you may have to create aurorae and themes folders).

4. Install the **QtCurve Style**. From bash: `cp ${DIR}/Other/QtCurve_theme/ElegantBreeze.qtcurve ~/.kde4/share/apps/QtCurve/` (You may have to create QtCurve directory). Then, chose ElegantBreeze from QtCurve styles.

5. Install the **Icons pack**. From bash: `cp -r ${DIR}/Other/Icons/flattr-icons-kde ~/.kde4/share/icons/flattr-icons-kde`. Then, choose Plasma Next from Icons menu (in System Settings) (you can also install **plasma-next-icons** in the same way, it's up to you)

6. Install the **Colorscheme**. From bash: `cp ${DIR}/Other/Colorscheme/ElegantBreeze.colorscheme ~/.kde4/share/apps/color-schemes/`. Then, choose ElegantBreeze from Colors menu (in System Settings)

7. Install the **Plasma Theme**. From bash: `cp -r ${DIR}/Other/Plasma_theme/Evolvere ~/.kde4/share/apps/desktoptheme/Evolvere`. Enable it from the Desktop Theme menu (in System Settings)

8. Install the **Cursor Theme**. From bash: `cp -r ${DIR}/Other/MouseCursor_theme/Breeze ~/.icons/Breeze`

9. Install **Wallpaper** contained in ${DIR}/Other/Wallpapers folder.

Please, notice that your ~/.kde4 folder could be ~/.kde instead, depending on your Distro.

About this theme
==============
I'm a newbie with Inkscape and KDE Theming. If you notice any problem, please, open an issue report here on Github.
If you have a patch/improovement, please make a pull request.

Credits
------
* KDE Team for the Breeze Cursor and for the Min/Max/Close icons.
* Evolvere's autor for his awesome work
* Flattr icons creator. Give a look to his work! :D
* The guys who created the QtCurve style, the ColorScheme and the Icons pack. I didn't find your nicknames, guys!
* The author of the wallpaper. Unfortunately, I don't remember where i found it :(

License
------
ElegantBreeze Aurorae Theme released under GNUGPLv3 license. The other components, contained in folder 'Other' are released under their own license. For any license question/complain, please contact me through email or filling an issue here on GitHub.

Screenshots
==============
![Screenshot1](/Screenshot1.png)

Changelog
==============

v 1.0
------
* First commit

v 1.0.1
------
* Added Flattr-icons

v 1.1
------
* Thinner title bar
* Tinner border
* Fixed some bugs
* Changed the focus rectangle to dotted
* flattr icons are now default
* Added an install bash script for a simple installation

v 1.1.1
------
* Added a suggested wallpaper (manual installation)

v 1.1.2
------
* Flatter popups and tooltips (removed round corners)
* Removed the dotted focus rectangle.
* Added links to patched QtCurve.