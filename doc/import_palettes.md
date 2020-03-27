[← Back to Home](/README.md)

Next: [Applying a palette to an image color map](/doc/set_color_map.md)

## Importing palettes into GIMP

Clone this git repo, or download the zipfile for the [latest
release](https://github.com/pilaf/liero-palettes/releases).

Look for the folder `palettes/gimp` and copy all .gpl (GIMP palette) files into
your GIMP profile folder:

* In Windows/GIMP 2.10:
  `C:\Users\{your-username}\AppData\Roaming\GIMP\2.10\palettes`
* In Linux/GIMP 2.10: `/home/{your-username}/.config/GIMP/2.10/palettes`
* In macOS/GIMP 2.10: `/Users/{your-username}/Library/GIMP/2.10/palettes` or `/Users/{your-username}/Library/Application Support/GIMP/2.10/palettes`

⚠️ NOTE: if you're on a different version of GIMP your profile folder will likely
be elsewhere

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

