* [Home](/README.md)
* [Introduction to Liero maps and GIMP](/doc/introduction.md)
* [Importing palettes into GIMP](/doc/import_palettes.md)
* [Applying a palette to an image color map](/doc/set_color_map.md)
* [Opening Liero levels in GIMP](/doc/open_lev_file.md)
* Exporting to Liero level format in GIMP
* [Tips on editing Liero levels in GIMP](/doc/editing_tips.md)

## Exporting to Liero level format (.lev file) in GIMP

### Checks

Before exporting your Liero level it's important to make sure your image file
has the following characteristics:

* Indexed 256-color mode
* 504&times;350 image dimensions

If your file doesn't meet these criteria Liero will fail to load your exported
.lev file.

You don't need to worry about merging your layers down, GIMP will merge them on
its own when you export.

### Exporting

Go to `File` → `Export As...`

![Export As...](/screenshots/export-as-menu.png)

In the Export Image dialog select `Raw image data` as the file type, and then
manually change the extension of your file to .lev.

NOTE: It's important to select the file type *before* you change the file
extension, as otherwise GIMP will change it back to .data.

![Export Image](/screenshots/export-dialog.png)

Once you click `Export` GIMP will warn you that the file extension doesn't
match, click on `Save` anyway.

In the **Export Image as Raw Data** dialog leave all settings in their defaults
and click `Export`.

![Export Image](/screenshots/export-as-raw-dialog.png)

Now your .lev file is ready to load into Liero/WebLiero.
