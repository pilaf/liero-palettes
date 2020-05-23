* [Home](/README.md)
* [Importing palettes into GIMP](/doc/import_palettes.md)
* [Applying a palette to an image color map](/doc/set_color_map.md)
* [Opening Liero levels in GIMP](/doc/open_lev_file.md)
* [Exporting to Liero level format in GIMP](/doc/save_lev_file.md)
* Tips on editing Liero levels in GIMP

## Tips on editing Liero maps in GIMP

### Layers

GIMP has pretty good layer support, so make use of it, that is - don't edit
your map as a flat image. GIMP takes care of flattening your image when you
export your .lev anyway.

Keep your layers separated by material as much as possible. For instance, have
your background layer be just background material, then use separate layers for
solid rock and dirt materials on top of that. Using layers this way will allow
you to change the layout of your map without having to redraw the background
when you move a platform around.

If you have many layers try labeling meaningful and easy-to-identify names, and
change the layers' color tags to symbolize the main material each layer uses.
For instance use a gray color tag for solid rock layers, brown tag for dirt,
etc.

![Labeled layers](/screenshots/labeled-layers.png)

### Use the Pencil Tool to edit pixels

GIMP has many tools you can use to draw directly on your image. However, since
Liero maps are essentially palette-based pixel art, it's better to limit
yourself to the *Pencil Tool* and avoid others like the Paintbrush or the
Airbrush. Unlike the Pencil Tool, those other tools apply fuzzy opacity to
stroke edges, which while looking great in GIMP, will not be carried over to
your final .lev, limiting your control over the final product.

![Tool fuzziness](/screenshots/tool-fuzziness.png)

In the above screenshot, the two smudges at the top were painted with the
Paintbrush and Airbrush tools respectively, while the bottom one was painted
with the Pencil Tool (all three using the same brush and stroke size settings).
While the two top ones look great in GIMP, that fuzziness will be lost when
exporting to .lev, with unexpected results. The bottom one however will look
exactly the same in the .lev.

### Enable Hard Edge when using the Eraser Tool

The Eraser Tool behaves like the Paintbrush by default, but it can be turned
to work like the Pencil by enabling the *Hard Edge* option in the tool options
pane, so make sure you do.

### Use Ctrl-click to quickly pick colors from the image

While drawing on the image it's often far quicker to pick a color from the
image itself than from the palette, or sometimes you just want to grab an
exact color. The Color Picker Tool allows you to do just that, but you don't
need to select it from the toolbox each time, instead you can just hold Ctrl
(or Cmd in macOS) while using the Pencil Tool, and it will turn into the
Color Picker until you release the key.
