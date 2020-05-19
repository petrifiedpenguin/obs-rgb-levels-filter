# obs-rgb-levels-filter
An OBS Studio filter to adjust RGB levels

## Compiling on Linux
```
git clone https:?????
cd obs-rgb-levels-filter
mkdir build && cd build
cmake -DLIBOBS_INCLUDE_DIR="...path to libobs source directory..." -DLIBOBS_LIB="...path to libobs.so file..." -DCMAKE_INSTALL_PREFIX=/usr ..
make -j4
sudo make install
```
