# eastray-setup

Script to download DOS extender and freeware EASTRAY raytracer and set up wrapper script to run EASTRAY from the command line via [DOSBox](https://www.dosbox.com).

Running `bash download.sh`, a sub folder `eastraydownload` is going to be created. `eastray.sh` inside that folder can be used to launch EASTRAY.

Syntax: `eastray.sh [-v] path/scene.ray`

The optional parameter `-v` shows the progress on raytraced scanlines; leaving it out no DOSBox window will be opened and EASTRAY will run silently.
