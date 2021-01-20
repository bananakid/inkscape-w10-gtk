# Windows 10 Light Mode Theme for Inkscape 1.1α

**Version:** 0.1.1

**Release:** 20.01.2021

**Description:** Quick essential fixes to default Adwaita GTK 3.24.24 theme to better match Windows 10 Light Mode

![Preview](https://user-images.githubusercontent.com/17095595/105144704-7598e400-5b1f-11eb-89e7-93ee0a6c6d28.png)

![Preview](https://user-images.githubusercontent.com/17095595/105144716-7b8ec500-5b1f-11eb-8d16-ee692bd5dfa2.PNG)

![Preview](https://user-images.githubusercontent.com/17095595/105144726-7df11f00-5b1f-11eb-89e1-144a9642cdeb.PNG)

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
5. Optionally, install transparent color UI image by copying 
   `remove-color.png` to `%ProgramFiles%\Inkscape\share\inkscape\pixmaps` 
   
**Release Notes**
- Theme is based on Adwaita GTK 3.24.24 compact theme's Sass source code
- Comments regarding most UI elements were added under // Default to modified
  Adwaita theme's  source code
- Adwaita theme's code modification made with no new lines (for easier updating)
- Unused Adwaita theme's elements were disabled in source code, not erased 
  (for easier tweaking)
- Complete source code is provided in corresponding folder for anyone interested
- Release 0.1.1 tested with Windows 10 version 1607 and 1809
- Release 0.1.1 doesn't match default Windows 10 colors for buttons,
  this may be added later on as an option
- Release 0.1.1 has thicker scrollbars and rulers than 0.1
  (Inkscape 1.1α related, may be fixed in later releases)
- Dark Mode theme may be added later on
- Please report issues or insights how to make it better
- Please refer to [Inkscape 1.0 Theming Guide](https://github.com/bananakid/inkscape-w10-gtk/blob/master/Inkscape%201.0%20Theming%20Guide.md) to understand Inkscape theming

**Licensing:** Feel free to redistribute, modify and include it in future releases of Inkscape

**Download:** [GitHub](https://github.com/bananakid/inkscape-w10-gtk/)

**P.S.** Previews of Windows 10 Light Mode Theme 0.1 for Inkscape 1.0:
- https://user-images.githubusercontent.com/17095595/81500319-ecbc7e00-92ea-11ea-9233-0aae1d264d80.PNG
- https://user-images.githubusercontent.com/17095595/81500320-ed551480-92ea-11ea-84bf-450e2176ee2f.PNG
- https://user-images.githubusercontent.com/17095595/81500317-eb8b5100-92ea-11ea-9e25-496f32b675ee.PNG
