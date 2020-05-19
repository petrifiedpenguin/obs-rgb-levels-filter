# obs-rgb-levels-filter
A simple OBS Studio filter to adjust RGB levels. 

I made this in order to fix a poor quality webcam image, for which the 
built-in OBS color-correction filter was inadequate.

Tested with OBS 25.0.8 running on Ubuntu 18.04.04 (x86_64).

## Compiling on Linux
You will have installed the obs-studio source files.

Set OBS_SRC_DIR to obs-studio source directory (e.g. /usr/local/src/obs-studio)
and LIBOBS_LIB to full path to libobs.so (e.g. /usr/lib/libobs.so)

```
git clone https:?????
cd obs_rgb_levels_filter
mkdir build && cd build
cmake -DOBS_SRC_DIR="...path to obs-studio source directory..." \
  -DLIBOBS_LIB="...path to libobs.so file..." -DCMAKE_INSTALL_PREFIX=/usr ..
make -j4
sudo make install
```

## Other platforms

I don't have access to a suitable machine to test this, but it should compile on
Windows/Mac (you may have to edit some paths in CMakeLists.txt for Windows)

