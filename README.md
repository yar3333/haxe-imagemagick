# ImageMagick haxelib

Installation:

    haxelib install ImageMagick

Then include this in your hxml files:

    -lib ImageMagick

You will need to ensure the appropriate `ndll` for your platform is in your `$NEKOPATH`.

### Compiling the NDLL

* Clone the sources:  
  `hg clone https://jasononeil@bitbucket.org/yar3333/haxe-imagemagick`
* Ensure you have the dev libraries installed. On Ubuntu:  
  `apt-get install libmagickcore-dev libmagickwand-dev neko-dev`.
* Edit `build/Makefile`, changing path to ImageMagick header files on your machine, if needed.  Eg `/usr/include/ImageMagick`.
* Build:  
  `make`
* Copy the ndll to your neko path:  
  `sudo cp library/ndll/Linux64/nMagick.ndll /usr/lib/neko/`

### Contribution guidelines

* Pull requests welcome