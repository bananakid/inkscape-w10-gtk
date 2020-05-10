# Windows 10 Light Mode Theme for Inkscape 1.0

**Version:** 0.1

**Release:** 10.05.2020

**Description:** Quick essential fixes to default Adwaita GTK 3.24.14 theme to better match Windows 10 Light Mode

**Bonus:** Compiled compact variation of Adwaita GTK 3.24.17 default theme is provided as a bonus

![Preview](https://user-images.githubusercontent.com/17095595/81500319-ecbc7e00-92ea-11ea-9233-0aae1d264d80.PNG)

![Preview](https://user-images.githubusercontent.com/17095595/81500320-ed551480-92ea-11ea-84bf-450e2176ee2f.PNG)

![Preview](https://user-images.githubusercontent.com/17095595/81500317-eb8b5100-92ea-11ea-9e25-496f32b675ee.PNG)

**Installation**
1. Copy entire folder `Windows 10 Light Mode`
   to folder `%ProgramFiles%\Inkscape\share\themes`
   or
   to folder `%UserProfile%\AppData\Local\Themes`
2. Launch Inkscape and select theme `Windows 10 Light Mode`
   using menu `Edit > Preferences > Interface > Theme`
   from drop-down menu under `Change GTK theme`,
   then close and relauch Inkscape
3. Optionally, specify icon settings to match previews using
   `Edit > Preferences > Interface > Theme` > `Icon theme` > `multicolor`,
   check `Use symbolic icons`, uncheck `Use default colors for icons`,
   set main icons color to `RGBA 343a40ff` and all highlighs colors to `RGBA 6d7881ff`
4. Optionally, install compact main toolbar and compact ruler 
   configuration files (as seen in preview) by copying `style.css` 
   and `toolbar-commands.ui` from `Toolbar & Ruler` folder 
   to `%ProgramFiles%\Inkscape\share\inkscape\ui`
   
**Release Notes**
- Theme is based on Adwaita GTK 3.24.14 theme's Sass source code
- Comments regarding most UI elements were added to modified Adwaita theme's source code
- Adwaita theme's code modification made with no new lines (for easier updating)
- Unused Adwaita theme's elements were disabled in source code, not erased (for easier tweaking)
- Complete source code is provided in corresponding folder for anyone interested
- Current theme appears to work correctly with Windows 10 version 1607 and 1809
- Theme doesn't match default Windows 10 colors for buttons, this may be added later on as an option
- Dark Mode theme may be added later on (feel free to compile draft version using gtk-dark.scss)
- Inkscape 1.0 released with Adwaita GTK 3.24.17 theme, however this theme
  was developed in Inkscape 1.0 RC1 which featured Adwaita GTK 3.24.14 theme,
  there appeared no notable differences between GTK 3.24.14 and 3.24.17
- Please report issues or insights how to make it better

**Licensing:** Feel free to redistribute, modify and include it in future releases of Inkscape

**Download:** [GitHub](https://github.com/bananakid/inkscape-w10-gtk/blob/master/Windows%2010%20Light%20Mode%20Theme%200.1%20for%20Inkscape%201.0.7z)
