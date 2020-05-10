# Inkscape 1.0 Theming Guide

Quick writeup for Windows users who may want to develop or tweak Inkscape themes using GTK and Sass. This may work similarly for Linux and gayOS

**Note:** Inkscape installation directory is meant to be `C:\Program Files\Inkscape` (bin, share and other folders go to this folder)

1. View `C:\Program Files\Inkscape\lib\gtk-3.0\immodules.cache` using your web browser

2. Take note of GTK version in `# Created by (...) from gtk+-3.24.14` line (3.24.14 for Inkscape 1.0RC1, 3.24.17 for Inkscape 1.0)

3. Go to GitHub and download corresponding release of GTK, i.e. https://github.com/GNOME/gtk/releases/tag/3.24.14 or https://github.com/GNOME/gtk/releases/tag/3.24.17

4. Unzip downloaded archive and navigate to `%Unzip_Destination_Folder%\gtk-3.24.14\gtk-3.24.14\gtk\theme\Adwaita`

5. Adwaita folder contains sources for compiling Adwaita theme used by Inkscape, copy this folder to your working folder, i.e. `C:\Users\User\Downloads\My Inkscape Theme Project`. Adwaita is the default and the most complete GTK 3 theme to date and it's quite common to modify it to get different appearence for OS or application 

6. Inside your working folder rename `_colors.scss`, `_colors-public.scss`, `_common.scss`, `_drawing.scss` to `colors.scss`, `colors-public.scss`, `common.scss`, `drawing.scss` and rename `gtk-contained.scss` to `gtk.scss`, `gtk-contained-dark.scss` to `gtk-dark.scss`

7. You may delete all files in your working Adwaita folder except:
- `assets` folder
- `colors.scss`
- `colors-public.scss`
- `common.scss`
- `drawing.scss`
- `gtk.scss`
- `gtk-dark.scss`

6. Download command-line Dart Sass compiler for SCSS files from https://github.com/sass/dart-sass/releases (some releases come without Windows-compatible executables, find and download one with `-windows-ia32.zip` or `-windows-x64.zip` in file name)

7. Unzip downloaded archive to `C:\Program Files\Dart Sass` (make sure file `sass.bat` and folder `src` go directly in `Dart Sass` folder with no sub-folders)

8. Right-click your Computer in Windows Explorer sidebar > click `Properties` > click `Advanced system settings` (on the left) > click `Environment Variable`s > Select `Path` variable > click `Edit` > click `New` > type in `C:\Program Files\Dart Sass` > click OK in every dialog. This makes sure you will be able to use `sass` command in Command Prompt with no extra steps

9. Create destination theme folders for your theme so Inkscape would recognize it at `C:\Program Files\Inkscape\share\themes\My Inkscape Theme\GTK-3.0` or at `%UserProfile%\AppData\Local\Themes\%YourThemeName%\GTK-3.0\*.*`

10. Copy assets folder from your working Adwaita folder to `C:\Program Files\Inkscape\share\themes\My Inkscape Theme\GTK-3.0\assets`

10. Compile SCSS files of Adwaita using Command Prompt command (use right-click on folder > `Copy as path` to get paths):
sass "%UserProfile\Documents\%YourThemeProjectFolder%\gtk.scss" "%ProgramFiles%\Inkscape\share\themes\%YourThemeName%\GTK-3.0\gtk.css"

11. Run Inkscape and select `%YourThemeName%` in Preferences. It should look exactly as default theme.

12. Close Inkscape; modify SCSS files in `%YourThemeProjectFolder%` folder; recompile it using sass command from Command Prompt (press up arrow on keyboard); open Inkscape to see changes.

13. To test if everything is set up correctly, edit common.scss on line 15 and set theme to be 'compact' (smaller buttons, etc.) — you should notice difference right away.

**Reference:** [Inkscape Wiki Theming Help](http://wiki.inkscape.org/wiki/index.php/Release_notes/1.0#Theme_selection)
