# Liero palettes

This repo contains a number of color palettes useful for editing Liero maps.

It also contains some Ruby code used to export and manipulate said palettes.

The rest of this README explains how to use those palettes to edit Liero maps
using GIMP.

## Importing palettes into GIMP

Clone this git repo, or download the zipfile for the [latest
release](https://github.com/pilaf/liero-palettes/releases).

Look for the folder `palettes/gimp` and copy all .gpl (GIMP palette) files into
your GIMP profile folder:

* In Windows/GIMP 2.10:
  `C:\Users\{your-username}\AppData\Roaming\GIMP\2.10\palettes`
* In Linux/GIMP 2.10: `/home/{your-username}/.config/GIMP/2.10/palettes`
* In macOS/GIMP 2.10: `/Users/{your-username}/Library/GIMP/2.10/palettes`

(NOTE: if you're on a different version of GIMP your profile folder will likely
be elsewhere)

Then run GIMP, or if you already had a running instance open the Palettes
dialog with `Windows -> Dockable Dialogs -> Palettes`

![Open Palettes dockable dialog](/screenshots/palettes-dockable.png)

Then right-click on the palettes tab and select `Refresh Palettes`

![Refresh Palettes in GIMP](/screenshots/refresh-palettes.png)

### Alternate method (manually importing palettes one by one)

Open the Palettes dialog with `Windows -> Dockable Dialogs -> Palettes`

![Open Palettes dockable dialog](/screenshots/palettes-dockable.png)

Once in the palettes dialog, right click on the palettes list and select
`Import Palette...`

Select the `Palette file` option in the import dialog and look for a .lpl file
to import.

![Import Palette](/screenshots/import-palette.png)

## Applying a palette as an image color map

First make sure your image is in indexed mode. If it's not, go to `Image ->
Mode -> Indexed`

![Indexed mode](/screenshots/mode-indexed-menu.png)

And once in the Indexed Color Conversion dialog select "Use custom palette" and
pick the palette you want, it will be applied as your color map.

If your image was already indexed, you can swap the color map with a palette by
going to `Colors -> Map -> Set Colormap...`

![Set colormap](/screenshots/set-colormap.png)

And then pick the palette you want.
