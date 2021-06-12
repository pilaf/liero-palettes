* [Home](/README.md)
* [Introduction to Liero maps and GIMP](/doc/introduction.md)
* [Importing palettes into GIMP](/doc/import_palettes.md)
* Applying a palette to an image color map
* [Opening Liero levels (.lev files) in GIMP](/doc/open_lev_file.md)
* [Exporting to Liero level format in GIMP](/doc/save_lev_file.md)
* [Tips on editing Liero levels in GIMP](/doc/editing_tips.md)

## Applying a palette to an image color map

Once you have the Liero palettes imported into GIMP you'll want to apply them
to your image's color map. The color map, also known as the color index or
palette index, is the 256-color palette that's embedded in the image and limits
the colors that image can show. An image that has a color map is said to be
"indexed".

### Starting from an RGB-mode image

If you're image not yet indexed (i.e. in RGB mode), then go to `Image` → `Mode`
→ `Indexed` to convert it.

![Indexed mode](/screenshots/mode-indexed-menu.png)

Once in the Indexed Color Conversion dialog select "Use custom palette" and
pick the palette you want (usually "Liero full unique" if you downloaded the
palettes from this guide), it will be applied as your color map.

⚠️ Warning: make sure the "Remove unused and duplicate colors from colormap"
checkbox is unchecked during this step.

![Indexed color conversion](/screenshots/indexed-color-conversion.png)

### Starting from an indexed mode image

If your image was already indexed, you can swap the color map with a palette by
going to `Colors` → `Map` → `Set Colormap...`

![Set colormap](/screenshots/set-colormap-menu.png)

And then pick the palette you want (usually "Liero full unique").

![Set colormap](/screenshots/set-colormap-dialog.png)
