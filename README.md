# obs-rgb-levels-filter
A simple OBS Studio filter to adjust RGB levels.

## Compiling on Linux
You will have installed and compiled obs-studio source.

Set LIBOBS_INCLUDE_DIR to obs-studio source directory (e.g. /usr/local/src/obs-studio)
and LIBOBS_INCLUDE_DIR to full path to libobs.so (e.g. /usr/lib/libobs.so or 
/usr/local/src/obs-studio/build/libobs/libobs.so)

```
git clone https:?????
cd obs_rgb_levels_filter
mkdir build && cd build
cmake -DLIBOBS_INCLUDE_DIR="...path to obs-studio source directory..." \
  -DLIBOBS_LIB="...path to libobs.so file..." -DCMAKE_INSTALL_PREFIX=/usr ..
make -j4
sudo make install
```
