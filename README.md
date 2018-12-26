# eastray-setup

Script to download DOS extender and freeware EASTRAY raytracer (originally developed for the [FM Towns](https://en.wikipedia.org/wiki/FM_Towns)) and set up wrapper script to run EASTRAY from the command line via [DOSBox](https://www.dosbox.com).

Running `bash download.sh`, a sub folder `eastraydownload` is going to be created. `eastray.sh` inside that folder can be used to launch EASTRAY.

Syntax: `eastray.sh [-v] path/scene.ray`

The optional parameter `-v` shows the progress on raytraced scanlines; leaving it out no DOSBox window will be opened and EASTRAY will run silently.

## TIFF files
EASTRAY can read and write both 32K and 16.7M color TIFF images. 32K color TIFFs were commonly used on the [FM Towns](https://en.wikipedia.org/wiki/FM_Towns) and can be converted to and from PNG with [tiff32k2png and png2tiff32k](https://github.com/v-joe/tiff32k). For high-quality picture output from EASTRAY, 16.7M color TIFF images are recommended; corresponding 24-bit output can be set in EASTRAY scene files via
```
output_mode
  24
   0 ;
output outputfile.tif
```
