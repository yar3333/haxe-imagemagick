# ImageMagick haxe library

### Installation:
```shell
haxelib install ImageMagick
```

Then include this in your hxml files:
```
-lib ImageMagick
```

You will need to ensure the appropriate `*.ndll` for your platform is in your `$NEKOPATH`.

### ImageMagick versions

* Windows: need `CORE_RL_wand_.dll` and dependencies from `ImageMagick-6.6.2-Q16`
* Linux: need `libMagickWand.so.5` from `libmagickwand5` package


### How to update (recompile) the NDLL

* Download or clone the sources:
	```shell
	hg clone https://bitbucket.org/yar3333/haxe-imagemagick
	```
* Ensure you have the dev libraries installed. On Ubuntu:  
	```shell
	apt-get install libmagickcore-dev libmagickwand-dev neko-dev
	```
* Edit `build/Makefile`, changing path to ImageMagick header files on your machine, if needed (`/usr/include/ImageMagick`)
* Goto `build` folder and run:  
	```shell
	make
	```
* Result NDLL file must appeare in `library/ndll/PLATFORM`


### Contribution guidelines

* Pull requests welcome
