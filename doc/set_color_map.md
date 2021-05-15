* [Home](/README.md)
* [Introduction to Liero maps and GIMP](/doc/introduction.md)
* [Importing palettes into GIMP](/doc/import_palettes.md)
* Applying a palette to an image color map
* [Opening Liero levels (.lev files) in GIMP](/doc/open_lev_file.md)
* [Exporting to Liero level format in GIMP](/doc/save_lev_file.md)
* [Tips on editing Liero levels in GIMP](/doc/editing_tips.md)

## Applying a palette to an image color map

First make sure your image is in indexed mode. If it's not, go to
`Image` → `Mode` → `Indexed`

![Indexed mode](/screenshots/mode-indexed-menu.png)

Once in the Indexed Color Conversion dialog select "Use custom palette" and
pick the palette you want (usually "Liero full unique" if you downloaded the
palettes from this guide), it will be applied as your color map.

⚠️ Warning: make sure the "Remove unused and duplicate colors from colormap"
checkbox is unchecked during this step.

![Indexed color conversion](/screenshots/indexed-color-conversion.png)

If your image was already indexed, you can swap the color map with a palette by
going to `Colors` → `Map` → `Set Colormap...`

![Set colormap](/screenshots/set-colormap-menu.png)

And then pick the palette you want (usually "Liero full unique").

![Set colormap](/screenshots/set-colormap-dialog.png)
