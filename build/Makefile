include Makefile-platform
include Makefile-ndll

PROJECT=nMagick

ifeq ($(PLATFORM),Windows)
	CCFLAGS+= -I original-windows
	LDFLAGS+= original-windows\VisualMagick\lib\CORE_RL_wand_.lib 
else
	CCFLAGS+= -I/usr/include/ImageMagick
	LDFLAGS+= -lMagickWand
endif 

