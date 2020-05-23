* [Home](/README.md)
* Introduction to Liero maps and GIMP
* [Importing palettes into GIMP](/doc/import_palettes.md)
* [Applying a palette to an image color map](/doc/set_color_map.md)
* [Opening Liero levels in GIMP](/doc/open_lev_file.md)
* [Exporting to Liero level format in GIMP](/doc/save_lev_file.md)
* [Tips on editing Liero levels in GIMP](/doc/editing_tips.md)

## Introduction to Liero maps and GIMP

### The Liero level format (.lev)

Being a classic DOS game, Liero uses 256-color palettes for its maps (also
called levels).  Liero map files themselves (files with .lev extension) are
just a string of exactly 176,400 bytes, each byte representing a color in the
map. Maps are always 504 pixels wide by 350 pixels high, hence the file size
(504&times;350 = 176,400).

Liero map files don't include the color palette itself, which means if you want
to edit a Liero map in GIMP or any other graphics editor you need to load the
palette separetely. Read the [next chapter](/doc/import_palettes.mod) of this
tutorial to learn how to that in GIMP.

Each color in the palette has different material properties in the game.
Materials are:

* Background (the area where worms move)
* Solid rock
* Dirt (diggable/destructible)
* Specials (e.g. material where bullets can go through but worms can't, or
  vice-versa)

The palettes in this repo include a full palette with all colors (used to apply
as the palette for the file), but also smaller palettes with just subsets of
the full one, separated by material type, so that you don't need to remember
which color does what by heart when editing your map.

### GIMP

GIMP is a free/open-source graphics editor similar to Photoshop and available
for Windows, Linux and macOS. You can download it from
[gimp.org](https://www.gimp.org/).

While GIMP is not specifically designed to work with palette-based pixel art,
it works fairly well for that purpose. It also allows you to load and save .lev
files (although with a few extra steps).

The rest of this tutorial focuses on using GIMP for editing Liero maps.
