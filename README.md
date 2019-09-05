# Liero palettes

This repo contains a number of color palettes useful for editing Liero maps.

It also contains some Ruby code used to export and manipulate said palettes.

The rest of this README explains how to use those palettes to edit Liero maps
using GIMP.

## Importing palettes into GIMP

Open the Palettes dialog with:

```
Windows -> Dockable Dialogs -> Palettes
```

Once in the palettes dialog, right click on the palettes list and select
`Import Palette...`.

Select the `Palette file` option in the import dialog and look for a .lpl file
to import.

## Applying a palette as an image color map

First make sure your image is in 256-color indexed mode. If it's not, go to:

```
Image -> Mode -> Indexed
```

And once in the Indexed Color Conversion dialog select "Use custom palette" and
pick the palette you want, it will be applied as your color map.

If your image was already indexed, you can swap the color map with a palette by
going to:

```
Colors -> Map -> Set Colormap...
```

And then pick the palette you want.
