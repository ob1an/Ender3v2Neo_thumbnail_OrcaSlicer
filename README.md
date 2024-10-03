# Ender3v2Neo_thumbnail_OrcaSlicer
This is a script to generate the right formatting for the my Ender3 printer with OrcaSlicer



This script is an adaptation and mix of these two :
https://github.com/fifonik/ElegooNeptuneThumbnailPrusaMod
https://github.com/KenHuffman/UltimakerCuraScripts/tree/main

This is not yet cleaned so read the file at your own risk.
You can refer to the original scripts to install or replicate how I use it.


# How I set it up

I created a python virtual environment to be sure, but the requirements are quite low.

#### How to configure OrcaSlicer:
Printer Settings / Basic information / G-code thumbnails -- 200x200/JPG
Print Settings / Others / Post-processing Scripts - specify path to python env and script : /path/to/.env/bin/python /path/to/Ender3V2Neo_thumbnail_from_OrcaSlicer.py

#### Printing :
The modified text on the image is :
on the left :
- filament used weight
- filament cost
on the right :
- print height of the piece
- layer height
- layers count


I tested it for Ender3v2 Neo only. Maybe some minor changes are needed for other models, I will try to clean and refactor the script to make it easier.